<script lang="ts">
    import { onMount } from "svelte";
    import { fly, fade } from "svelte/transition";
    import { cubicOut } from "svelte/easing";
    import SlideTitle from "$lib/components/slides/SlideTitle.svelte";
    import SlideIntro from "$lib/components/slides/SlideIntro.svelte";
    import SlideProfile from "$lib/components/slides/SlideProfile.svelte";
    import SlideTimeline from "$lib/components/slides/SlideTimeline.svelte";
    import SlideKillChain from "$lib/components/slides/SlideKillChain.svelte";
    import SlideStats from "$lib/components/slides/SlideStats.svelte";
    import SlideImpact from "$lib/components/slides/SlideImpact.svelte";
    import SlideConclusion from "$lib/components/slides/SlideConclusion.svelte";

    let currentSlide = 0;
    let direction = 1; // 1 for next, -1 for prev

    const slides = [
        SlideTitle,
        SlideIntro,
        SlideProfile,
        SlideTimeline,
        SlideKillChain,
        SlideStats,
        SlideImpact,
        SlideConclusion,
    ];

    function next() {
        if (currentSlide < slides.length - 1) {
            direction = 1;
            currentSlide++;
        }
    }

    function prev() {
        if (currentSlide > 0) {
            direction = -1;
            currentSlide--;
        }
    }

    function handleKeydown(e: KeyboardEvent) {
        if (e.key === "ArrowRight" || e.key === " ") {
            e.preventDefault();
            next();
        }
        if (e.key === "ArrowLeft") {
            e.preventDefault();
            prev();
        }
    }

    onMount(() => {
        window.addEventListener("keydown", handleKeydown);
        return () => window.removeEventListener("keydown", handleKeydown);
    });
</script>

<svelte:head>
    <title>PROJECT: LAZARUS // {currentSlide + 1}</title>
</svelte:head>

<main class="fixed inset-0 bg-obsidian overflow-hidden select-none font-body">
    {#key currentSlide}
        <div
            in:fly={{
                x: 100 * direction,
                duration: 800,
                easing: cubicOut,
                opacity: 0,
            }}
            out:fade={{ duration: 400 }}
            class="absolute inset-0"
        >
            <div class="w-full h-full relative overflow-hidden">
                <svelte:component this={slides[currentSlide]} />
            </div>
        </div>
    {/key}

    <!-- Top Status Bar -->
    <div
        class="fixed top-0 w-full px-12 py-6 z-[60] flex justify-between items-center pointer-events-none"
    >
        <div class="flex items-center gap-12">
            <div class="hidden md:flex flex-col items-end">
                <p
                    class="text-[10px] text-slate-500 font-mono tracking-widest leading-none"
                >
                    OPERATION PHASE
                </p>
                <p
                    class="text-xs text-blue-500 font-mono font-bold leading-none uppercase"
                >
                    {currentSlide === 0
                        ? "Infiltration"
                        : currentSlide === slides.length - 1
                          ? "Exfiltration"
                          : "Active Analysis"}
                </p>
            </div>
            <div class="h-12 w-px bg-slate-800"></div>
            <div class="flex flex-col items-end">
                <p
                    class="text-[10px] text-slate-500 font-mono tracking-widest leading-none"
                >
                    FRAME INDEX
                </p>
                <p class="text-xs text-white font-mono font-bold leading-none">
                    0{currentSlide + 1} / 0{slides.length}
                </p>
            </div>
        </div>
    </div>

    <!-- Navigation Hub (Bottom Right) -->
    <div class="fixed bottom-12 right-12 z-[60] flex items-center gap-4">
        <div class="flex flex-col items-end mr-4">
            <p
                class="text-[10px] text-slate-600 font-mono tracking-widest uppercase mb-1"
            >
                Navigation Hub
            </p>
            <div class="h-0.5 w-12 bg-blue-500/20 rounded-full"></div>
        </div>

        <button
            on:click={prev}
            disabled={currentSlide === 0}
            aria-label="Previous Slide"
            class="w-14 h-14 glass-panel rounded-full flex items-center justify-center text-slate-500 hover:text-white hover:border-blue-500/50 disabled:opacity-10 transition-all active:scale-90"
        >
            <i class="fas fa-chevron-left text-lg" aria-hidden="true"></i>
        </button>

        <button
            on:click={next}
            disabled={currentSlide === slides.length - 1}
            aria-label="Next Slide"
            class="w-14 h-14 bg-blue-600 rounded-full flex items-center justify-center text-white shadow-[0_0_20px_rgba(37,99,235,0.4)] hover:bg-blue-500 hover:scale-105 transition-all active:scale-95 disabled:opacity-10"
        >
            <i class="fas fa-chevron-right text-lg" aria-hidden="true"></i>
        </button>
    </div>

    <!-- Global Progress Bar (Bottom) -->
    <div class="fixed bottom-0 left-0 w-full h-[5px] bg-slate-900 z-[60]">
        <div
            class="h-full bg-gradient-to-r from-blue-600 to-blue-400 shadow-[0_0_10px_rgba(59,130,246,0.5)] transition-all duration-700 ease-out"
            style="width: {((currentSlide + 1) / slides.length) * 100}%"
        ></div>
    </div>
</main>

<style>
    :global(body) {
        margin: 0;
        background-color: #020617;
        cursor: crosshair;
    }
</style>
