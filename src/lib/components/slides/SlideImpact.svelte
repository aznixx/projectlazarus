<script>
    import GridBackground from "$lib/components/GridBackground.svelte";
</script>

<div class="slide-view relative w-full h-full overflow-hidden">
    <GridBackground />

    <div
        class="relative z-10 flex flex-col h-full p-8 md:p-16 lg:p-20 gap-8 lg:gap-12 w-full"
    >
        <!-- Header -->
        <h2
            class="text-[4rem] md:text-[6.5rem] lg:text-[9rem] font-black text-white font-space tracking-tighter leading-none italic"
        >
            HET <span class="text-teal-glow">GEVAAR</span>
        </h2>

        <div class="flex-1 grid grid-cols-1 lg:grid-cols-2 gap-8 lg:gap-16">
            <!-- Left: Impact Column -->
            <div class="space-y-8 lg:space-y-12">
                <div class="flex items-center gap-6">
                    <div
                        class="h-1.5 bg-crimson-glow/30 flex-1 rounded-full"
                    ></div>
                    <span
                        class="text-lg md:text-2xl font-black font-space tracking-[0.6em] uppercase italic text-crimson-glow"
                        >GEVOLG</span
                    >
                    <div
                        class="h-1.5 bg-crimson-glow/30 w-12 rounded-full"
                    ></div>
                </div>

                <div class="space-y-6 lg:space-y-8">
                    <div
                        class="glass-panel-premium p-6 md:p-8 rounded-[1.5rem] border-l-[8px] border-crimson-glow hover:bg-crimson-glow/[0.1] transition-all duration-700 group shadow-[0_30px_60px_rgba(0,0,0,0.6)]"
                    >
                        <div class="flex gap-6 items-center">
                            <div
                                class="w-16 h-16 rounded-[1.5rem] bg-crimson-glow/15 flex items-center justify-center text-crimson-glow shrink-0 group-hover:scale-110 transition-transform shadow-[0_0_30px_rgba(255,0,60,0.3)]"
                            >
                                <i class="fas fa-power-off text-2xl md:text-3xl"
                                ></i>
                            </div>
                            <div>
                                <h3
                                    class="text-2xl md:text-4xl font-black font-space uppercase italic text-white mb-1"
                                >
                                    PLAT
                                </h3>
                                <p
                                    class="text-lg md:text-xl text-slate-intel leading-tight"
                                >
                                    Banken gaan <span
                                        class="text-white italic font-bold"
                                        >uit</span
                                    >.
                                </p>
                            </div>
                        </div>
                    </div>

                    <div
                        class="glass-panel-premium p-6 md:p-8 rounded-[1.5rem] border-l-[8px] border-crimson-glow hover:bg-crimson-glow/[0.1] transition-all duration-700 group shadow-[0_30px_60px_rgba(0,0,0,0.6)]"
                    >
                        <div class="flex gap-6 items-center">
                            <div
                                class="w-16 h-16 rounded-[1.5rem] bg-crimson-glow/15 flex items-center justify-center text-crimson-glow shrink-0 group-hover:scale-110 transition-transform shadow-[0_0_30px_rgba(255,0,60,0.3)]"
                            >
                                <i
                                    class="fas fa-sack-dollar text-2xl md:text-3xl"
                                ></i>
                            </div>
                            <div>
                                <h3
                                    class="text-2xl md:text-4xl font-black font-space uppercase italic text-white mb-1"
                                >
                                    ROOF
                                </h3>
                                <p
                                    class="text-lg md:text-xl text-slate-intel leading-tight"
                                >
                                    Miljarden aan <span
                                        class="text-white italic font-bold"
                                        >geld</span
                                    > weg.
                                </p>
                            </div>
                        </div>
                    </div>

                    <div
                        class="glass-panel-premium p-6 md:p-8 rounded-[1.5rem] border-l-[8px] border-crimson-glow hover:bg-crimson-glow/[0.1] transition-all duration-700 group shadow-[0_30px_60px_rgba(0,0,0,0.6)]"
                    >
                        <div class="flex gap-6 items-center">
                            <div
                                class="w-16 h-16 rounded-[1.5rem] bg-crimson-glow/15 flex items-center justify-center text-crimson-glow shrink-0 group-hover:scale-110 transition-transform shadow-[0_0_30px_rgba(255,0,60,0.3)]"
                            >
                                <i class="fas fa-landmark text-2xl md:text-3xl"
                                ></i>
                            </div>
                            <div>
                                <h3
                                    class="text-2xl md:text-4xl font-black font-space uppercase italic text-white mb-1"
                                >
                                    STRAF
                                </h3>
                                <p
                                    class="text-lg md:text-xl text-slate-intel leading-tight"
                                >
                                    Bedrijven krijgen <span
                                        class="text-white italic font-bold"
                                        >boetes</span
                                    >.
                                </p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Right: Mitigation Column -->
            <div class="space-y-8 lg:space-y-7">
                <div class="flex items-center gap-6">
                    <div
                        class="h-1.5 bg-teal-glow/30 flex-1 rounded-full"
                    ></div>
                    <span
                        class="text-lg md:text-2xl font-black font-space tracking-[0.8em] uppercase italic text-teal-glow"
                        >HULP</span
                    >
                    <div class="h-1.5 bg-teal-glow/30 w-12 rounded-full"></div>
                </div>

                <div
                    class="absolute -top-[15rem] -right-[15rem] w-[400px] h-[400px] bg-teal-glow/10 rounded-full blur-[100px]"
                ></div>

                <div
                    class="glass-panel-premium mt-12 p-6 md:p-7 rounded-[1.5rem] border-l-[8px] border-crimson-glow hover:bg-crimson-glow/[0.1] transition-all duration-700 group shadow-[0_30px_60px_rgba(0,0,0,0.6)]"
                >
                    <div class="flex gap-6 md:gap-10 items-center group">
                        <div
                            class="w-16 h-16 md:w-20 md:h-20 bg-white/5 rounded-[1.5rem] flex items-center justify-center text-teal-glow border-2 border-white/5 group-hover:intel-border group-hover:bg-teal-glow group-hover:text-obsidian transition-all duration-500 shadow-[0_0_40px_rgba(0,245,255,0.1)]"
                        >
                            <i class="fas fa-lock text-2xl md:text-3xl"></i>
                        </div>
                        <div class="space-y-1">
                            <h4
                                class="text-white font-black text-2xl md:text-4xl uppercase tracking-tighter italic leading-none"
                            >
                                SLOT
                            </h4>
                            <p
                                class="text-lg md:text-xl text-slate-intel leading-tight italic"
                            >
                                Gebruik altijd <span
                                    class="text-white font-black">MFA</span
                                >.
                            </p>
                        </div>
                    </div>
                </div>
                <div
                    class="glass-panel-premium p-6 md:p-7 rounded-[1.5rem] border-l-[8px] border-crimson-glow hover:bg-crimson-glow/[0.1] transition-all duration-700 group shadow-[0_30px_60px_rgba(0,0,0,0.6)]"
                >
                    <div class="flex gap-6 md:gap-10 items-center group">
                        <div
                            class="w-16 h-16 md:w-20 md:h-20 bg-white/5 rounded-[1.5rem] flex items-center justify-center text-teal-glow border-2 border-white/5 group-hover:intel-border group-hover:bg-teal-glow group-hover:text-obsidian transition-all duration-500 shadow-[0_0_40px_rgba(0,245,255,0.1)]"
                        >
                            <i class="fas fa-network-wired text-2xl md:text-3xl"
                            ></i>
                        </div>
                        <div class="space-y-1">
                            <h4
                                class="text-white font-black text-2xl md:text-4xl uppercase tracking-tighter italic leading-none"
                            >
                                MUUR
                            </h4>
                            <p
                                class="text-lg md:text-xl text-slate-intel leading-tight italic"
                            >
                                Beveilig je <span class="text-white font-black"
                                    >data</span
                                >.
                            </p>
                        </div>
                    </div>
                </div>

                <div
                    class="glass-panel-premium p-6 md:p-7 rounded-[1.5rem] border-l-[8px] border-crimson-glow hover:bg-crimson-glow/[0.1] transition-all duration-700 group shadow-[0_30px_60px_rgba(0,0,0,0.6)]"
                >
                    <div class="flex gap-6 md:gap-10 items-center group">
                        <div
                            class="w-16 h-16 md:w-20 md:h-20 bg-white/5 rounded-[1.5rem] flex items-center justify-center text-teal-glow border-2 border-white/5 group-hover:intel-border group-hover:bg-teal-glow group-hover:text-obsidian transition-all duration-500 shadow-[0_0_40px_rgba(0,245,255,0.1)]"
                        >
                            <i class="fas fa-bell text-2xl md:text-3xl"></i>
                        </div>
                        <div class="space-y-1">
                            <h4
                                class="text-white font-black text-2xl md:text-4xl uppercase tracking-tighter italic leading-none"
                            >
                                ALARM
                            </h4>
                            <p
                                class="text-lg md:text-xl text-slate-intel leading-tight italic"
                            >
                                Check <span class="text-white font-black"
                                    >vreemde</span
                                > zaken.
                            </p>
                        </div>
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
</style>
