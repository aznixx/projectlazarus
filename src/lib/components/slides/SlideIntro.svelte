<script>
    import GridBackground from "$lib/components/GridBackground.svelte";
</script>

<div class="slide-view relative w-full h-full overflow-hidden">
    <GridBackground />

    <div
        class="relative z-10 w-full h-full flex flex-col p-6 md:p-10 lg:p-12 gap-8 lg:gap-12"
    >
        <!-- Header: Edge to Edge -->
        <div
            class="flex mt-12 flex-col lg:flex-row justify-between items-end border-b-8 border-white/5 pb-16 gap-12"
        >
            <div class="space-y-6 text-center lg:text-left">
                <h2
                    class="text-[4rem] md:text-[5.5rem] lg:text-[7rem] font-black text-white font-space tracking-tighter leading-none italic"
                >
                    HET <span class="text-teal-glow">PLAN</span>
                </h2>
            </div>
            <div
                class="hidden lg:block text-right font-mono text-xl text-slate-intel tracking-[0.5em] opacity-30"
            >
                STATUS: ACTIEF<br />
                VEILIGHEID: MAXIMAAL
            </div>
        </div>

        <!-- content Grid: Spreading to fill -->
        <div
            class="flex-1 grid grid-cols-1 md:grid-cols-3 gap-8 lg:gap-12 pb-16"
        >
            <!-- Box 1 -->
            <div
                class="glass-panel-premium rounded-[2rem] p-8 lg:p-10 intel-border transition-all duration-700 hover:translate-y-[-10px] flex flex-col justify-between group"
            >
                <div>
                    <div
                        class="w-16 h-16 lg:w-20 lg:h-20 bg-teal-glow/10 rounded-[1.5rem] flex items-center justify-center text-teal-glow mb-6 group-hover:bg-teal-glow group-hover:text-obsidian transition-all duration-500 shadow-[0_0_40px_rgba(0,245,255,0.2)]"
                    >
                        <i class="fas fa-mask text-3xl lg:text-4xl"></i>
                    </div>
                    <h3
                        class="text-4xl lg:text-[3.5rem] font-black text-white mb-6 font-space italic"
                    >
                        WIE
                    </h3>
                    <p
                        class="text-lg lg:text-2xl text-slate-intel leading-relaxed"
                    >
                        Een leger van <span class="text-white font-bold"
                            >6.000 hackers</span
                        >.
                    </p>
                </div>
                <div
                    class="pt-8 mb- border-t-2 border-white/5 flex items-center justify-between"
                >
                    <span
                        class="text-base font-mono text-slate-intel/40 tracking-[0.4em] uppercase"
                        >TEAM</span
                    >
                    <span class="text-teal-glow font-mono font-black text-3xl"
                        >121</span
                    >
                </div>
            </div>

            <!-- Box 2 -->
            <div
                class="glass-panel-premium rounded-[3rem] p-12 lg:p-16 border-2 border-white/5 transition-all duration-700 hover:translate-y-[-15px] flex flex-col justify-between group"
            >
                <div>
                    <div
                        class="w-16 h-16 lg:w-20 lg:h-20 bg-crimson-glow/10 rounded-[1.5rem] flex items-center justify-center text-crimson-glow mb-6 group-hover:bg-crimson-glow group-hover:text-white transition-all duration-500 shadow-[0_0_40px_rgba(255,0,60,0.2)]"
                    >
                        <i class="fas fa-bolt-lightning text-3xl lg:text-4xl"
                        ></i>
                    </div>
                    <h3
                        class="text-4xl lg:text-[3.5rem] font-black text-white mb-6 font-space italic"
                    >
                        HOE
                    </h3>
                    <p
                        class="text-lg lg:text-2xl text-slate-intel leading-relaxed"
                    >
                        Inbreken via <span class="text-white font-bold"
                            >mail</span
                        >
                        en <span class="text-white font-bold">links</span>.
                    </p>
                </div>
                <div
                    class="pt-8 border-t-2 border-white/5 flex items-center justify-between"
                >
                    <span
                        class="text-base font-mono text-slate-intel/40 tracking-[0.4em] uppercase"
                        >RISICO</span
                    >
                    <span
                        class="text-crimson-glow font-mono font-black text-3xl"
                        >HOOG</span
                    >
                </div>
            </div>

            <!-- Box 3 -->
            <div
                class="glass-panel-premium rounded-[3rem] p-12 lg:p-16 border-2 border-white/5 transition-all duration-700 hover:translate-y-[-15px] flex flex-col justify-between group"
            >
                <div>
                    <div
                        class="w-16 h-16 lg:w-20 lg:h-20 bg-teal-glow/10 rounded-[1.5rem] flex items-center justify-center text-teal-glow mb-6 group-hover:bg-teal-glow group-hover:text-obsidian transition-all duration-500 shadow-[0_0_40px_rgba(0,245,255,0.2)]"
                    >
                        <i class="fas fa-coins text-3xl lg:text-4xl"></i>
                    </div>
                    <h3
                        class="text-4xl lg:text-[3.5rem] font-black text-white mb-6 font-space italic"
                    >
                        BUIT
                    </h3>
                    <p
                        class="text-lg lg:text-2xl text-slate-intel leading-relaxed"
                    >
                        Diefstal van <span class="text-white font-bold"
                            >Bitcoin</span
                        >
                        en <span class="text-white font-bold">geld</span>.
                    </p>
                </div>
                <div
                    class="pt-8 border-t-2 border-white/5 flex items-center justify-between"
                >
                    <span
                        class="text-base font-mono text-slate-intel/40 tracking-[0.4em] uppercase"
                        >FOCUS</span
                    >
                    <span class="text-teal-glow font-mono font-black text-3xl"
                        >CRYPTO</span
                    >
                </div>
            </div>

            <div class="flex w-300 h-300">
                <img src="../../../../static/images/suspects/sus1.png" alt="" />
            </div>
        </div>
    </div>
</div>

<style>
    .slide-view {
        background-color: #020205;
    }
</style>
