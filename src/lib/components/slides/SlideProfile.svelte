<script>
    import GridBackground from "$lib/components/GridBackground.svelte";
</script>

<div class="slide-view relative w-full h-full overflow-hidden">
    <GridBackground />

    <div
        class="relative z-10 grid grid-cols-1 xl:grid-cols-12 gap-6 md:gap-10 lg:gap-12 w-full h-full p-6 md:p-10 lg:p-12"
    >
        <!-- Left: Personality Dossier -->
        <div
            class="xl:col-span-8 flex flex-col justify-center space-y-12 lg:space-y-24"
        >
            <div class="space-y-8">
                <div class="flex items-center gap-8">
                    <div class="h-2 bg-slate-intel/20 w-24 rounded-full"></div>
                    <div
                        class="text-xl font-mono text-teal-glow tracking-[0.6em] uppercase"
                    >
                        DOSSIER
                    </div>
                    <div
                        class="h-2 bg-slate-intel/20 flex-1 rounded-full"
                    ></div>
                </div>
                <h2
                    class="text-[4rem] md:text-[5.5rem] lg:text-[7rem] font-black text-white font-space tracking-tighter leading-[0.8] italic"
                >
                    WIE IS<br />
                    <span class="text-teal-glow">LAZARUS?</span>
                </h2>
            </div>

            <!-- Intelligence Blocks -->
            <div class="grid grid-cols-1 sm:grid-cols-2 gap-8 lg:gap-16 pb-8">
                <div class="space-y-6 opacity-0 animate-fade-in-L1">
                    <h4
                        class="text-teal-glow/80 font-black uppercase text-xl tracking-[0.5em] font-space flex items-center gap-6 italic"
                    >
                        <span class="w-3 h-3 bg-teal-glow rounded-full"></span>
                        LEGER
                    </h4>
                    <p
                        class="text-lg lg:text-2xl text-slate-200 leading-tight glass-panel-premium p-6 lg:p-8 rounded-[1.5rem] border-l-[8px] border-teal-glow/40"
                    >
                        Geen amateurs, maar een <span
                            class="text-white font-bold italic"
                            >militaire eenheid</span
                        > van Noord-Korea.
                    </p>
                </div>
                <div class="space-y-6 opacity-0 animate-fade-in-L2">
                    <h4
                        class="text-teal-glow/80 font-black uppercase text-xl tracking-[0.5em] font-space flex items-center gap-6 italic"
                    >
                        <span class="w-3 h-3 bg-teal-glow rounded-full"></span>
                        ALIASSEN
                    </h4>
                    <div class="flex flex-wrap gap-4">
                        <span
                            class="px-6 py-3 bg-white/5 border-2 border-white/10 rounded-xl text-xl lg:text-2xl font-mono text-slate-intel font-black italic"
                            >APT38</span
                        >
                        <span
                            class="px-6 py-3 bg-white/5 border-2 border-white/10 rounded-xl text-xl lg:text-2xl font-mono text-slate-intel font-black italic"
                            >COBRA</span
                        >
                        <span
                            class="px-6 py-3 bg-white/5 border-2 border-white/10 rounded-xl text-xl lg:text-2xl font-mono text-slate-intel font-black italic"
                            >ZINC</span
                        >
                    </div>
                </div>
                <div class="space-y-6 opacity-0 animate-fade-in-L1">
                    <h4
                        class="text-teal-glow/80 font-black uppercase text-xl tracking-[0.5em] font-space flex items-center gap-6 italic"
                    >
                        <span class="w-3 h-3 bg-teal-glow rounded-full"></span>
                        EXPERTS
                    </h4>
                    <p
                        class="text-lg lg:text-2xl text-slate-200 leading-tight glass-panel-premium p-6 lg:p-10 h-32 rounded-[1.5rem] border-l-[8px] border-teal-glow/40"
                    >
                        Meer dan <span class="text-white font-bold italic"
                            >6.000 hackers</span
                        > wereldwijd actief.
                    </p>
                </div>
                <div class="space-y-6 opacity-0 animate-fade-in-L2">
                    <h4
                        class="text-teal-glow/80 font-black uppercase text-xl tracking-[0.5em] font-space flex items-center gap-6 italic"
                    >
                        <span class="w-3 h-3 bg-teal-glow rounded-full"></span>
                        TIJD
                    </h4>
                    <div
                        class="glass-panel-premium p-6 lg:p-11 rounded-[1.5rem] border-2 border-white/5 flex items-center justify-center"
                    >
                        <span
                            class="text-1xl lg:text-3xl font-black text-white font-space italic shadow-[0_0_30px_rgba(255,255,255,0.1)]"
                            >SINDS 2009</span
                        >
                    </div>
                </div>
            </div>
        </div>

        <!-- Right: Suspect Dossier -->
        <div class="xl:col-span-4 flex items-center justify-center p-4">
            <div
                class="w-full max-w-[300px] opacity-0 glass-panel-premium rounded-[2.5rem] p-6 lg:p-8 border-2 border-white/10 flex flex-col gap-4 overflow-hidden relative group animate-fade-in-L3 shadow-[0_0_50px_rgba(0,0,0,0.5)]"
            >
                <div
                    class="absolute top-0 right-0 p-6 font-mono text-[0.6rem] text-slate-intel/20"
                >
                    SECURE NODE: 771.02.XX
                </div>

                <div class="flex items-center justify-between mb-4">
                    <div class="flex flex-col">
                        <span
                            class="text-sm font-mono text-crimson-glow tracking-widest uppercase font-black"
                            >TOP SECRET</span
                        >
                        <span
                            class="text-[0.6rem] font-mono text-slate-intel/50"
                            >INTEL DOSSIER // UNIT 121</span
                        >
                    </div>
                </div>

                <div class="grid grid-rows-3 gap-3 flex-1">
                    <div
                        class="relative group/img overflow-hidden rounded-xl border-2 border-white/5 h-36 w-36 mx-auto"
                    >
                        <img
                            src="/images/suspects/sus1.png"
                            alt="Suspect 1"
                            class="w-36 h-36 object-cover grayscale brightness-50 contrast-125 group-hover/img:grayscale-0 group-hover/img:brightness-100 transition-all duration-700 scale-110 group-hover/img:scale-100"
                        />
                        <div
                            class="absolute inset-0 bg-gradient-to-t from-black/90 via-transparent to-transparent opacity-60"
                        ></div>
                        <div
                            class="absolute bottom-3 left-4 flex flex-col opacity-0 group-hover/img:opacity-100 transition-all duration-500 translate-y-2 group-hover/img:translate-y-0"
                        >
                            <span class="font-mono text-[0.5rem] text-teal-glow"
                                >SUBJECT ID</span
                            >
                            <span
                                class="font-mono text-xs text-white font-black"
                                >SUSPECT-1</span
                            >
                        </div>
                    </div>

                    <div
                        class="relative group/img overflow-hidden rounded-xl border-2 border-white/5 h-36 w-36 mx-auto"
                    >
                        <img
                            src="/images/suspects/sus2.png"
                            alt="Suspect 2"
                            class="w-36 h-36 object-cover grayscale brightness-50 contrast-125 group-hover/img:grayscale-0 group-hover/img:brightness-100 transition-all duration-700 scale-110 group-hover/img:scale-100"
                        />
                        <div
                            class="absolute inset-0 bg-gradient-to-t from-black/90 via-transparent to-transparent opacity-60"
                        ></div>
                        <div
                            class="absolute bottom-3 left-4 flex flex-col opacity-0 group-hover/img:opacity-100 transition-all duration-500 translate-y-2 group-hover/img:translate-y-0"
                        >
                            <span class="font-mono text-[0.5rem] text-teal-glow"
                                >SUBJECT ID</span
                            >
                            <span
                                class="font-mono text-xs text-white font-black"
                                >SUSPECT-2</span
                            >
                        </div>
                    </div>

                    <div
                        class="relative group/img overflow-hidden rounded-xl border-2 border-white/5 h-36 w-36 mx-auto"
                    >
                        <img
                            src="/images/suspects/sus3.png"
                            alt="Suspect 3"
                            class="w-36 h-36 object-cover grayscale brightness-50 contrast-125 group-hover/img:grayscale-0 group-hover/img:brightness-100 transition-all duration-700 scale-110 group-hover/img:scale-100"
                        />
                        <div
                            class="absolute inset-0 bg-gradient-to-t from-black/90 via-transparent to-transparent opacity-60"
                        ></div>
                        <div
                            class="absolute bottom-3 left-4 flex flex-col opacity-0 group-hover/img:opacity-100 transition-all duration-500 translate-y-2 group-hover/img:translate-y-0"
                        >
                            <span class="font-mono text-[0.5rem] text-teal-glow"
                                >SUBJECT ID</span
                            >
                            <span
                                class="font-mono text-xs text-white font-black"
                                >SUSPECT-3</span
                            >
                        </div>
                    </div>
                </div>

                <div
                    class="mt-4 pt-6 border-t border-white/10 group-hover:border-crimson-glow/30 transition-colors"
                >
                    <div class="flex justify-between items-center mb-2">
                        <span
                            class="text-[0.5rem] font-mono text-slate-intel/50 tracking-tighter uppercase"
                            >Signal Trace</span
                        >
                        <span
                            class="text-[0.5rem] font-mono text-crimson-glow animate-pulse"
                            >84% DEPTH</span
                        >
                    </div>
                    <div
                        class="h-1 w-full bg-crimson-glow/10 rounded-full overflow-hidden"
                    >
                        <div
                            class="h-full bg-crimson-glow w-[84%] animate-[shimmer_2s_infinite]"
                        ></div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</div>

<style>
    .slide-view {
        background-color: #020205;
    }

    @keyframes fade-in {
        from {
            opacity: 0;
            transform: translateY(60px);
        }
        to {
            opacity: 1;
            transform: translateY(0);
        }
    }

    .animate-fade-in-L1 {
        animation: fade-in 1.5s ease-out forwards;
    }
    .animate-fade-in-L2 {
        animation: fade-in 1.5s ease-out 0.6s forwards;
    }
    .animate-fade-in-L3 {
        animation: fade-in 1.5s ease-out 1.2s forwards;
    }
</style>
