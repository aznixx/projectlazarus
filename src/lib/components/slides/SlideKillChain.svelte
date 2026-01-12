<script>
    import GridBackground from "$lib/components/GridBackground.svelte";
</script>

<div class="slide-view relative w-full h-full overflow-hidden">
    <GridBackground />

    <div class="relative z-10 w-full h-full flex flex-col p-6 md:p-10 lg:p-12">
        <!-- Title Section -->
        <div class="text-center mb-6 md:mb-8">
            <div class="inline-flex items-center gap-8 mb-4">
                <div class="h-2 w-32 bg-teal-glow/20 rounded-full"></div>
                <span
                    class="text-xl md:text-3xl font-mono text-teal-glow tracking-[0.8em] uppercase italic font-black"
                    >METHODE</span
                >
                <div class="h-2 w-32 bg-teal-glow/20 rounded-full"></div>
            </div>
            <h2
                class="text-[4rem] md:text-[6.5rem] lg:text-[9rem] mt-6 font-black text-white italic font-space tracking-tighter leading-none"
            >
                DE <span
                    class="text-teal-glow shadow-[0_0_100px_rgba(0,245,255,0.4)] w-[20rem]"
                    >HACK</span
                >
            </h2>
        </div>

        <!-- diagram Row: filling the width -->
        <div
            class="flex-1 flex flex-col lg:flex-row items-center justify-between gap-8 lg:gap-6 w-full pb-12 md:pb-16"
        >
            <!-- Step 1 -->
            <div
                class="relative z-20 flex-1 flex flex-col items-center group w-full"
            >
                <div
                    class="w-16 h-16 md:w-20 md:h-20 glass-panel-premium rounded-[1.5rem] flex items-center justify-center text-teal-glow border-4 border-white/5 mb-6 group-hover:intel-border group-hover:scale-110 transition-all duration-700 shadow-[0_15px_30px_rgba(0,0,0,0.5)]"
                >
                    <i class="fas fa-envelope-open-text text-3xl md:text-5xl"
                    ></i>
                </div>
                <div
                    class="glass-panel-premium p-6 md:p-8 rounded-[2rem] border-2 border-white/5 text-center w-full min-h-[160px] flex flex-col justify-center relative group-hover:bg-teal-glow/[0.04] transition-colors"
                >
                    <h3
                        class="text-2xl md:text-4xl font-black text-white mb-4 font-space uppercase italic"
                    >
                        MAIL
                    </h3>
                    <p
                        class="text-xl md:text-2xl text-slate-intel leading-tight"
                    >
                        Valse mail met <span class="text-white font-bold italic"
                            >virus</span
                        >.
                    </p>
                    <div
                        class="absolute -bottom-2 left-1/2 -translate-x-1/2 w-24 h-2 bg-teal-glow opacity-0 group-hover:opacity-100 transition-opacity rounded-full shadow-[0_0_20px_#00f5ff]"
                    ></div>
                </div>
            </div>

            <!-- Step 2 -->
            <div
                class="relative z-20 flex-1 flex flex-col items-center lg:-translate-y-16 group w-full"
            >
                <div
                    class="w-16 h-16 md:w-20 md:h-20 glass-panel-premium rounded-[1.5rem] flex items-center justify-center text-teal-glow border-4 border-white/5 mb-6 group-hover:intel-border group-hover:scale-110 transition-all duration-700 shadow-[0_15px_30px_rgba(0,0,0,0.5)]"
                >
                    <i class="fas fa-file-shield text-3xl md:text-5xl"></i>
                </div>
                <div
                    class="glass-panel-premium p-6 md:p-8 rounded-[2rem] border-2 border-white/5 text-center w-full min-h-[160px] flex flex-col justify-center relative group-hover:bg-teal-glow/[0.04] transition-colors"
                >
                    <h3
                        class="text-2xl md:text-4xl font-black text-white mb-4 font-space uppercase italic"
                    >
                        MALWARE
                    </h3>
                    <p
                        class="text-xl md:text-2xl text-slate-intel leading-tight"
                    >
                        Geheime <span class="text-white font-bold italic"
                            >toegang</span
                        >.
                    </p>
                    <div
                        class="absolute -bottom-2 left-1/2 -translate-x-1/2 w-24 h-2 bg-teal-glow opacity-0 group-hover:opacity-100 transition-opacity rounded-full shadow-[0_0_20px_#00f5ff]"
                    ></div>
                </div>
            </div>

            <!-- Step 3 -->
            <div
                class="relative z-20 flex-1 flex flex-col items-center group w-full"
            >
                <div
                    class="w-16 h-16 md:w-20 md:h-20 glass-panel-premium rounded-[1.5rem] flex items-center justify-center text-teal-glow border-4 border-white/5 mb-6 group-hover:intel-border group-hover:scale-110 transition-all duration-700 shadow-[0_15px_30px_rgba(0,0,0,0.5)]"
                >
                    <i class="fas fa-vault text-3xl md:text-5xl"></i>
                </div>
                <div
                    class="glass-panel-premium p-6 md:p-8 rounded-[2rem] border-2 border-white/5 text-center w-full min-h-[160px] flex flex-col justify-center relative group-hover:bg-teal-glow/[0.04] transition-colors"
                >
                    <h3
                        class="text-2xl md:text-4xl font-black text-white mb-4 font-space uppercase italic"
                    >
                        ROOF
                    </h3>
                    <p
                        class="text-xl md:text-2xl text-slate-intel leading-tight"
                    >
                        Stelen van <span class="text-white font-bold italic"
                            >crypto</span
                        >.
                    </p>
                    <div
                        class="absolute -bottom-2 left-1/2 -translate-x-1/2 w-24 h-2 bg-teal-glow opacity-0 group-hover:opacity-100 transition-opacity rounded-full shadow-[0_0_20px_#00f5ff]"
                    ></div>
                </div>
            </div>

            <!-- Step 4 -->
            <div
                class="relative z-20 flex-1 flex flex-col items-center lg:-translate-y-16 group w-full"
            >
                <div
                    class="w-16 h-16 md:w-20 md:h-20 bg-crimson-glow/20 rounded-[1.5rem] flex items-center justify-center text-crimson-glow border-4 border-crimson-glow/40 mb-6 group-hover:bg-crimson-glow group-hover:text-white transition-all duration-700 shadow-[0_0_40px_rgba(255,0,60,0.4)]"
                >
                    <i class="fas fa-skull text-3xl md:text-5xl"></i>
                </div>
                <div
                    class="glass-panel-premium p-6 md:p-8 rounded-[2rem] border-4 border-crimson-glow/20 text-center w-full min-h-[160px] flex flex-col justify-center relative group-hover:bg-crimson-glow/[0.1] transition-colors"
                >
                    <h3
                        class="text-crimson-glow font-black uppercase text-2xl md:text-4xl mb-4 font-space italic"
                    >
                        GELD
                    </h3>
                    <p
                        class="text-xl md:text-2xl text-slate-intel leading-tight"
                    >
                        Miljarden voor <span class="text-white font-bold italic"
                            >wapens</span
                        >.
                    </p>
                    <div
                        class="absolute -bottom-2 left-1/2 -translate-x-1/2 w-24 h-2 bg-crimson-glow opacity-0 group-hover:opacity-100 transition-opacity rounded-full shadow-[0_0_20px_#ff003c]"
                    ></div>
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
