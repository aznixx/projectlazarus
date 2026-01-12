<script lang="ts">
    import { onMount } from "svelte";

    interface Particle {
        x: number;
        y: number;
        speedX: number;
        speedY: number;
        opacity: number;
        size: number;
    }

    let particles: Particle[] = [];
    const particleCount = 20;

    onMount(() => {
        particles = Array.from({ length: particleCount }).map(() => ({
            x: Math.random() * 100,
            y: Math.random() * 100,
            speedX: (Math.random() - 0.5) * 0.15,
            speedY: (Math.random() - 0.5) * 0.15,
            opacity: Math.random() * 0.5 + 0.2,
            size: Math.random() * 6 + 1,
        }));

        let frame: number;
        function animate() {
            particles = particles.map((p) => {
                p.x += p.speedX;
                p.y += p.speedY;

                // Wrap around
                if (p.x > 100) p.x = 0;
                if (p.x < 0) p.x = 100;
                if (p.y > 100) p.y = 0;
                if (p.y < 0) p.y = 100;

                return p;
            });
            frame = requestAnimationFrame(animate);
        }
        animate();
        return () => cancelAnimationFrame(frame);
    });
</script>

<div
    class="background-container absolute inset-0 overflow-hidden pointer-events-none z-0"
>
    <!-- Base Deep Background -->
    <div class="absolute inset-0 bg-obsidian"></div>

    <!-- Ultra-Fine Grid -->
    <div class="grid-overlay absolute inset-0 opacity-[0.07]"></div>

    <!-- Moving Data Particles -->
    {#each particles as p}
        <div
            class="absolute bg-teal-glow rounded-full shadow-[0_0_10px_#00f5ff] transition-opacity duration-1000"
            style="left: {p.x}%; top: {p.y}%; width: {p.size}px; height: {p.size}px; opacity: {p.opacity}"
        ></div>
    {/each}

    <!-- Scanning Beam from app.css -->
    <div class="beam-effect"></div>

    <!-- Radial Depth Vignette -->
    <div class="absolute inset-0 radial-depth"></div>

    <!-- Noise Texture Overlay (Global) -->
    <div class="noise-overlay"></div>
</div>

<style>
    .background-container {
        background-color: #020205;
    }

    .grid-overlay {
        background-image: linear-gradient(
                to right,
                rgba(0, 245, 255, 0.4) 1px,
                transparent 1px
            ),
            linear-gradient(
                to bottom,
                rgba(0, 245, 255, 0.4) 1px,
                transparent 1px
            );
        background-size: 80px 80px;
    }

    .radial-depth {
        background: radial-gradient(
            circle at 50% 50%,
            transparent 0%,
            rgba(2, 2, 5, 0.8) 100%
        );
    }

    @keyframes beam-sweep {
        0% {
            transform: translateY(-100%) rotate(0deg);
            opacity: 0;
        }
        50% {
            opacity: 0.05;
        }
        100% {
            transform: translateY(200%) rotate(0deg);
            opacity: 0;
        }
    }

    .beam-effect {
        position: absolute;
        width: 100%;
        height: 15vh;
        background: linear-gradient(
            to bottom,
            transparent,
            rgba(0, 245, 255, 0.3),
            transparent
        );
        animation: beam-sweep 15s infinite ease-in-out;
    }
</style>
