<script>
    import GridBackground from "$lib/components/GridBackground.svelte";
</script>

<div class="slide-view relative w-full h-full overflow-hidden">
    <GridBackground />

    <div class="relative z-10 w-full h-full flex flex-col p-6 md:p-10 lg:p-12">
        <!-- Header -->
        <div
            class="flex mt-12 flex-col lg:flex-row justify-between items-center lg:items-end border-b-8 border-white/10 pb-8 md:pb-12 gap-8 w-full"
        >
            <div class="text-center lg:text-left">
                <h2
                    class="text-[4rem] md:text-[6rem] lg:text-[8rem] font-black text-white font-space tracking-tighter leading-none italic"
                >
                    TIJD<span class="text-teal-glow">LIJN</span>
                </h2>
                <p
                    class="text-lg md:text-2xl font-mono text-slate-intel uppercase tracking-[0.8em] mt-4 italic"
                >
                    OPERATIE LOGBOEK // ARCHIEF
                </p>
            </div>
            <div
                class="intel-border glass-panel-premium px-8 py-4 rounded-[1.5rem] flex items-center gap-6 shadow-[0_0_60px_rgba(255,0,60,0.2)]"
            >
                <span
                    class="w-4 h-4 bg-crimson-glow rounded-full animate-pulse shadow-[0_0_20px_#ff003c]"
                ></span>
                <span
                    class="text-lg md:text-xl font-mono text-white tracking-[0.4em] uppercase font-black italic"
                    >LIVE</span
                >
            </div>
        </div>

        <!-- Timeline Chassis -->
        <div
            class="flex-1 relative flex flex-col lg:flex-row items-center justify-between px-4 md:px-8 lg:px-12 py-12 gap-16 lg:gap-0 w-full max-w-7xl mx-auto"
        >
            <!-- Main Line -->
            <div
                class="hidden lg:block absolute left-16 right-16 h-2 bg-gradient-to-r from-transparent via-teal-glow/50 to-transparent blur-sm"
            ></div>

            <!-- Event 1 -->
            <div
                class="relative flex flex-col items-center group w-full lg:w-auto"
            >
                <div
                    class="lg:absolute lg:-top-[14rem] w-full lg:w-[22rem] glass-panel-premium p-6 rounded-[2rem] border-2 border-white/10 opacity-100 lg:opacity-0 lg:translate-y-20 lg:group-hover:opacity-100 lg:group-hover:translate-y-0 transition-all duration-700 ease-out z-30 shadow-[0_40px_80px_rgba(0,0,0,0.8)]"
                >
                    <div class="flex justify-between items-center mb-4">
                        <span
                            class="text-sm font-mono text-teal-glow uppercase tracking-[0.4em] italic mb-2 font-black"
                            >SONY</span
                        >
                        <i class="fas fa-video text-teal-glow/30 text-2xl"></i>
                    </div>
                    <h3
                        class="text-2xl font-black text-white mb-2 font-space italic"
                    >
                        HACK
                    </h3>
                    <p class="text-lg text-slate-intel leading-tight">
                        Systemen <span class="text-white font-bold italic"
                            >kapot</span
                        >. Alles gestolen.
                    </p>
                </div>
                <div
                    class="hidden lg:block w-12 h-12 rounded-full bg-obsidian border-[6px] border-teal-glow shadow-[0_0_40px_#00f5ff] z-20 group-hover:scale-125 transition-all duration-500"
                ></div>
                <div class="mt-8 lg:mt-12 text-center">
                    <p
                        class="text-3xl md:text-4xl lg:text-5xl font-black text-white font-space italic tracking-tighter group-hover:text-teal-glow transition-colors"
                    >
                        2014
                    </p>
                </div>
            </div>

            <!-- Event 2 -->
            <div
                class="relative flex flex-col items-center group w-full lg:w-auto"
            >
                <div
                    class="mt-8 lg:mt-0 mb-8 lg:mb-12 text-center hidden lg:block"
                >
                    <p
                        class="text-3xl md:text-4xl lg:text-5xl font-black text-white font-space italic tracking-tighter group-hover:text-teal-glow transition-colors"
                    >
                        2017
                    </p>
                </div>
                <div
                    class="hidden lg:block w-12 h-12 rounded-full bg-obsidian border-[6px] border-teal-glow shadow-[0_0_40px_#00f5ff] z-20 group-hover:scale-125 transition-all duration-500"
                ></div>
                <div
                    class="lg:absolute lg:-bottom-[14rem] w-full lg:w-[22rem] glass-panel-premium p-6 rounded-[2rem] border-2 border-white/10 opacity-100 lg:opacity-0 lg:translate-y-[-40px] lg:group-hover:opacity-100 lg:group-hover:translate-y-0 transition-all duration-700 ease-out z-30 shadow-[0_40px_80px_rgba(0,0,0,0.8)]"
                >
                    <div class="flex justify-between items-center mb-4">
                        <span
                            class="text-sm font-mono text-crimson-glow uppercase tracking-[0.4em] italic mb-2 font-black"
                            >VIRUS</span
                        >
                        <i
                            class="fas fa-biohazard text-crimson-glow/30 text-2xl"
                        ></i>
                    </div>
                    <h3
                        class="text-2xl font-black text-white mb-2 font-space italic"
                    >
                        WANNACRY
                    </h3>
                    <p class="text-lg text-slate-intel leading-tight">
                        Wereldwijd alles <span
                            class="text-white font-bold italic">plat</span
                        >.
                    </p>
                </div>
                <div class="mt-8 lg:mt-12 text-center lg:hidden">
                    <p
                        class="text-3xl md:text-4xl lg:text-5xl font-black text-white font-space italic tracking-tighter group-hover:text-teal-glow transition-colors"
                    >
                        2017
                    </p>
                </div>
            </div>

            <!-- Event 3 -->
            <div
                class="relative flex flex-col items-center group w-full lg:w-auto"
            >
                <div
                    class="lg:absolute lg:-top-[14rem] w-full lg:w-[22rem] glass-panel-premium p-6 rounded-[2rem] border-2 border-white/10 opacity-100 lg:opacity-0 lg:translate-y-20 lg:group-hover:opacity-100 lg:group-hover:translate-y-0 transition-all duration-700 ease-out z-30 shadow-[0_40px_80px_rgba(0,0,0,0.8)]"
                >
                    <div class="flex justify-between items-center mb-4">
                        <span
                            class="text-sm font-mono text-teal-glow uppercase tracking-[0.4em] italic mb-2 font-black"
                            >BANK</span
                        >
                        <i class="fas fa-vault text-teal-glow/30 text-2xl"></i>
                    </div>
                    <h3
                        class="text-2xl font-black text-white mb-2 font-space italic"
                    >
                        ROOF
                    </h3>
                    <p class="text-lg text-slate-intel leading-tight">
                        <span class="text-white font-bold italic"
                            >$81 Miljoen</span
                        >
                        gestolen.
                    </p>
                </div>
                <div
                    class="hidden lg:block w-12 h-12 rounded-full bg-obsidian border-[6px] border-teal-glow shadow-[0_0_40px_#00f5ff] z-20 group-hover:scale-125 transition-all duration-500"
                ></div>
                <div class="mt-8 lg:mt-12 text-center">
                    <p
                        class="text-3xl md:text-4xl lg:text-5xl font-black text-white font-space italic tracking-tighter group-hover:text-teal-glow transition-colors"
                    >
                        2018
                    </p>
                </div>
            </div>

            <!-- Event 4 -->
            <div
                class="relative flex flex-col items-center group w-full lg:w-auto"
            >
                <div
                    class="mt-8 lg:mt-0 mb-8 lg:mb-12 text-center hidden lg:block"
                >
                    <p
                        class="text-3xl md:text-4xl lg:text-5xl font-black text-white font-space italic tracking-tighter group-hover:text-teal-glow transition-colors"
                    >
                        2022+
                    </p>
                </div>
                <div
                    class="hidden lg:block w-12 h-12 rounded-full bg-obsidian border-[6px] border-teal-glow shadow-[0_0_40px_#00f5ff] z-20 group-hover:scale-125 transition-all duration-500"
                ></div>
                <div
                    class="lg:absolute lg:-bottom-[14rem] w-full lg:w-[22rem] glass-panel-premium p-6 rounded-[2rem] border-2 border-white/10 opacity-100 lg:opacity-0 lg:translate-y-[-40px] lg:group-hover:opacity-100 lg:group-hover:translate-y-0 transition-all duration-700 ease-out z-30 shadow-[0_40px_80px_rgba(0,0,0,0.8)]"
                >
                    <div class="flex justify-between items-center mb-4">
                        <span
                            class="text-sm font-mono text-teal-glow uppercase tracking-[0.4em] italic mb-2 font-black"
                            >CRYPTO</span
                        >
                        <i
                            class="fas fa-bitcoin-sign text-teal-glow/30 text-2xl"
                        ></i>
                    </div>
                    <h3
                        class="text-2xl font-black text-white mb-2 font-space italic"
                    >
                        RECORD
                    </h3>
                    <p class="text-lg text-slate-intel leading-tight">
                        <span class="text-white font-bold italic"
                            >$625 Miljoen</span
                        > weg.
                    </p>
                </div>
                <div class="mt-8 lg:mt-12 text-center lg:hidden">
                    <p
                        class="text-6xl md:text-7xl lg:text-8xl font-black text-white font-space italic tracking-tighter group-hover:text-teal-glow transition-colors"
                    >
                        2022+
                    </p>
                </div>
            </div>
        </div>
    </div>
</div>

<style>
    .slide-view {
        background-color: #020205;
    }
</style>
