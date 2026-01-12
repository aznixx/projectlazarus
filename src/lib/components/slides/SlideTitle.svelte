<script>
    import GridBackground from "$lib/components/GridBackground.svelte";
</script>

<div class="slide-view relative w-full h-full overflow-hidden">
    <GridBackground />

    <!-- Hero Layout: Spanning the whole screen -->
    <div
        class="relative z-10 w-full h-full flex flex-col lg:flex-row items-center justify-between p-8 md:p-12 lg:p-16"
    >
        <!-- Left Side: Massive Text -->
        <div
            class="flex-1 space-y-12 lg:space-y-24 text-center lg:text-left z-20"
        >
            <div class="space-y-6 md:space-y-8">
                <h1
                    class="text-[4rem] sm:text-[6rem] md:text-[8rem] lg:text-[10rem] xl:text-[12rem] font-black text-white tracking-[-0.08em] leading-[0.7] font-space italic opacity-0 animate-reveal-title"
                >
                    PROJECT<br />
                    <span
                        class="text-teal-glow drop-shadow-[0_0_100px_rgba(0,245,255,0.6)]"
                        >LAZARUS</span
                    >
                </h1>
                <div
                    class="h-3 w-48 md:w-64 bg-teal-glow rounded-full opacity-0 animate-reveal-bar mx-auto lg:mx-0 shadow-[0_0_30px_#00f5ff]"
                ></div>
            </div>
        </div>

        <!-- Right Side: Massive Logo pinned to right -->
        <div
            class="relative flex-none w-[250px] h-[250px] sm:w-[350px] sm:h-[350px] lg:w-[450px] lg:h-[450px] xl:w-[500px] xl:h-[500px] flex items-center justify-center"
        >
            <!-- Layers -->
            <div
                class="absolute inset-0 border-[4px] border-teal-glow/10 rounded-full animate-spin-ultra-slow"
            ></div>
            <div
                class="absolute inset-20 border-2 border-white/5 rounded-full animate-reverse-spin-slow"
            ></div>
            <div
                class="absolute inset-0 bg-teal-glow/10 rounded-full blur-[180px] animate-pulse-glow"
            ></div>

            <!-- Logo -->
            <div
                class="relative z-100 w-full h-full p-36 lg:p-24 opacity-0 animate-zoom-in"
            >
                <div
                    class="absolute inset-0 bg-crimson-glow/10 rounded-full blur-[120px]"
                ></div>
                <img
                    src="/lazarus_logo.png"
                    alt="Lazarus"
                    class="w-full h-full object-contain drop-shadow-[0_0_100px_rgba(255,0,60,0.5)] transition-transform duration-1000 hover:scale-110"
                />
            </div>
        </div>
    </div>

    <!-- Edge Decorations -->
    <div
        class="absolute bottom-12 left-12 font-mono text-sm text-slate-intel/20 tracking-[1em] uppercase z-20"
    >
        PYONGYANG // NORTH KOREA
    </div>
    <div
        class="absolute top-12 right-12 font-mono text-sm text-slate-intel/20 tracking-[1em] uppercase z-20"
    >
        UNIT 121 // RGB
    </div>
</div>

<style>
    .slide-view {
        background-color: #020205;
    }

    @keyframes reveal-title {
        0% {
            transform: translateY(100px) skewY(5deg);
            opacity: 0;
            filter: blur(40px);
        }
        100% {
            transform: translateY(0) skewY(0);
            opacity: 1;
            filter: blur(0);
        }
    }

    @keyframes reveal-bar {
        0% {
            transform: scaleX(0);
            opacity: 0;
        }
        100% {
            transform: scaleX(1);
            opacity: 1;
        }
    }

    @keyframes fade-in {
        0% {
            opacity: 0;
            transform: translateY(40px);
        }
        100% {
            opacity: 1;
            transform: translateY(0);
        }
    }

    @keyframes zoom-in {
        0% {
            opacity: 0;
            transform: scale(0.6) rotate(-20deg);
            filter: brightness(0);
        }
        100% {
            opacity: 1;
            transform: scale(1) rotate(0);
            filter: brightness(1);
        }
    }

    @keyframes spin-ultra-slow {
        from {
            transform: rotate(0deg);
        }
        to {
            transform: rotate(360deg);
        }
    }

    @keyframes reverse-spin-slow {
        from {
            transform: rotate(360deg);
        }
        to {
            transform: rotate(0deg);
        }
    }

    .animate-reveal-title {
        animation: reveal-title 1.6s cubic-bezier(0.2, 0.8, 0.2, 1) 0.2s
            forwards;
    }

    .animate-reveal-bar {
        animation: reveal-bar 1.5s cubic-bezier(0.2, 0.8, 0.2, 1) 1.5s forwards;
        transform-origin: left;
    }

    .animate-zoom-in {
        animation: zoom-in 2s cubic-bezier(0.2, 0.8, 0.2, 1) 0.5s forwards;
    }

    .animate-spin-ultra-slow {
        animation: spin-ultra-slow 60s linear infinite;
    }
    .animate-reverse-spin-slow {
        animation: reverse-spin-slow 50s linear infinite;
    }
    .animate-pulse-glow {
        animation: pulse-glow 8s infinite;
    }

    @keyframes pulse-glow {
        0%,
        100% {
            opacity: 0.1;
            transform: scale(1);
        }
        50% {
            opacity: 0.4;
            transform: scale(1.2);
        }
    }
</style>
