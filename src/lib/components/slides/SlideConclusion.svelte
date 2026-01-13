<script>
    import GridBackground from "$lib/components/GridBackground.svelte";
</script>

<div class="slide-view relative w-full h-full overflow-hidden">
    <GridBackground />

    <div class="relative z-10 flex flex-col h-full w-full p-8 md:p-16 lg:p-20">
        <!-- Main Conclusion Section -->
        <div
            class="flex-1 flex flex-col justify-center items-center text-center space-y-4"
        >
            <div class="space-y-8 lg:space-y-12 animate-reveal-final">
                <div class="flex items-center justify-center gap-10 mb-8">
                    <div class="h-2 w-32 bg-teal-glow/30 rounded-full"></div>
                    <span
                        class="text-xl md:text-2xl font-mono text-teal-glow tracking-[1em] uppercase italic font-black"
                        >EINDE</span
                    >
                    <div class="h-2 w-32 bg-teal-glow/30 rounded-full"></div>
                </div>
                <h2
                    class="text-[5rem] md:text-[8rem] lg:text-[10rem] xl:text-[12rem] font-black text-white font-space tracking-tighter leading-none italic"
                >
                    HET <span class="text-teal-glow shadow-[0_0_150px_#00f5ff]"
                        >EINDE</span
                    >
                </h2>
                <div
                    class="h-2 w-32 md:w-[200px] bg-teal-glow rounded-full mx-auto shadow-[0_0_60px_#00f5ff] mt-8"
                ></div>
            </div>

            <div
                class="grid grid-cols-1 md:grid-cols-3 gap-12 w-full mt-2 ml-60 opacity-0 animate-fade-in-L3"
            >
                <div
                    class="space-y-2 w-100 glass-panel-premium p-6 lg:p-3 rounded-[2rem] border-2 border-white/5 shadow-[0_40px_80px_rgba(0,0,0,0.8)] group hover:intel-border transition-all"
                >
                    <p
                        class="text-base md:text-lg text-slate-intel uppercase tracking-[0.6em] font-mono font-black italic"
                    >
                        TIJD
                    </p>
                    <p
                        class="text-2xl md:text-3xl font-black text-white font-space italic"
                    >
                        2009 — NU
                    </p>
                </div>
                <div
                    class="space-y-2 w-100 glass-panel-premium p-6 lg:p-3 rounded-[2rem] border-2 border-white/5 shadow-[0_40px_80px_rgba(0,0,0,0.8)] group hover:intel-border transition-all shadow-[0_0_60px_rgba(0,245,255,0.2)]"
                >
                    <p
                        class="text-base md:text-lg text-slate-intel uppercase tracking-[0.6em] font-mono font-black italic"
                    >
                        RISICO
                    </p>
                    <p
                        class="text-2xl md:text-3xl font-black text-teal-glow font-space uppercase italic"
                    >
                        MAXIMAAL
                    </p>
                </div>
                <div
                    class="space-y-2 w-100 glass-panel-premium p-6 lg:p-3 rounded-[2rem] border-2 border-white/5 shadow-[0_40px_80px_rgba(0,0,0,0.8)] group hover:intel-border transition-all"
                >
                    <p
                        class="text-base md:text-lg text-slate-intel uppercase tracking-[0.6em] font-mono font-black italic"
                    >
                        STATUS
                    </p>
                    <p
                        class="text-2xl md:text-3xl font-black text-crimson-glow font-space uppercase italic"
                    >
                        ACTIEF
                    </p>
                </div>
            </div>

            <p
                class="text-2xl md:text-3xl lg:text-4xl text-slate-intel font-black max-w-full leading-tight opacity-0 animate-fade-in-delayed px-12 uppercase tracking-widest italic pt-8"
            >
                LAZARUS IS EEN <span
                    class="text-white border-b-[6px] border-teal-glow pb-1"
                    >GEVAAR</span
                >.
            </p>
        </div>

        <!-- Sources: MASSIVE FOOTER -->
        <div
            class="glass-panel-premium p-6 lg:p-8 rounded-[2rem] border-2 border-white/10 flex flex-col gap-6 mt-12 min-w-max shadow-[0_60px_120px_rgba(0,0,0,0.9)]"
        >
            <div class="flex items-center gap-10">
                <span
                    class="text-xl text-slate-intel/50 font-mono uppercase tracking-[1em] font-black italic"
                    >BRONNEN</span
                >
                <div class="h-2 bg-white/10 flex-1 rounded-full"></div>
            </div>
            <div class="grid grid-cols-2 md:grid-cols-4 gap-8 lg:gap-16">
                <a
                    href="https://attack.mitre.org/groups/G0032/"
                    target="_blank"
                    class="flex items-center gap-6 p-6 hover:bg-white/5 rounded-[2.5rem] transition-all duration-300 group"
                >
                    <div
                        class="w-16 h-16 bg-teal-glow/10 rounded-[1.5rem] flex items-center justify-center text-teal-glow group-hover:scale-125 transition-transform shadow-[0_0_40px_rgba(0,245,255,0.2)]"
                    >
                        <i class="fas fa-database text-3xl"></i>
                    </div>
                    <div>
                        <p
                            class="text-xl text-white font-black font-space uppercase tracking-widest italic"
                        >
                            MITRE
                        </p>
                        <p class="text-sm text-slate-intel font-mono">G0032</p>
                    </div>
                </a>
                <a
                    href="https://www.fbi.gov"
                    target="_blank"
                    class="flex items-center gap-6 p-6 hover:bg-white/5 rounded-[2.5rem] transition-all duration-300 group"
                >
                    <div
                        class="w-16 h-16 bg-teal-glow/10 rounded-[1.5rem] flex items-center justify-center text-teal-glow group-hover:scale-125 transition-transform shadow-[0_0_40px_rgba(0,245,255,0.2)]"
                    >
                        <i class="fas fa-building-shield text-3xl"></i>
                    </div>
                    <div>
                        <p
                            class="text-xl text-white font-black font-space uppercase tracking-widest italic"
                        >
                            FBI
                        </p>
                        <p class="text-sm text-slate-intel font-mono">
                            ARCHIEF
                        </p>
                    </div>
                </a>
                <a
                    href="https://www.cisa.gov"
                    target="_blank"
                    class="flex items-center gap-6 p-6 hover:bg-white/5 rounded-[2.5rem] transition-all duration-300 group"
                >
                    <div
                        class="w-16 h-16 bg-teal-glow/10 rounded-[1.5rem] flex items-center justify-center text-teal-glow group-hover:scale-125 transition-transform shadow-[0_0_40px_rgba(0,245,255,0.2)]"
                    >
                        <i class="fas fa-tower-broadcast text-3xl"></i>
                    </div>
                    <div>
                        <p
                            class="text-xl text-white font-black font-space uppercase tracking-widest italic"
                        >
                            CISA
                        </p>
                        <p class="text-sm text-slate-intel font-mono">ALERTS</p>
                    </div>
                </a>
                <a
                    href="https://www.picussecurity.com/resource/blog/lazarus-group-apt38-explained-timeline-ttps-and-major-attacks"
                    target="_blank"
                    class="flex items-center gap-6 p-6 hover:bg-white/5 rounded-[2.5rem] transition-all duration-300 group"
                >
                    <div
                        class="w-16 h-16 bg-teal-glow/10 rounded-[1.5rem] flex items-center justify-center text-teal-glow group-hover:scale-125 transition-transform shadow-[0_0_40px_rgba(0,245,255,0.2)]"
                    >
                        <i class="fas fa-book text-3xl"></i>
                    </div>
                    <div>
                        <p
                            class="text-xl text-white font-black font-space uppercase tracking-widest italic"
                        >
                            PICUS SECURITY
                        </p>
                        <p class="text-sm text-slate-intel font-mono">INFO</p>
                    </div>
                </a>
            </div>
        </div>
    </div>
</div>

<style>
    .slide-view {
        background-color: #020205;
    }

    @keyframes reveal-final {
        from {
            transform: scale(0.9);
            opacity: 0;
            filter: blur(50px);
        }
        to {
            transform: scale(1);
            opacity: 1;
            filter: blur(0);
        }
    }

    @keyframes fade-in {
        from {
            opacity: 0;
            transform: translateY(80px);
        }
        to {
            opacity: 1;
            transform: translateY(0);
        }
    }

    .animate-reveal-final {
        animation: reveal-final 2s cubic-bezier(0.2, 0.8, 0.2, 1) forwards;
    }

    .animate-fade-in-delayed {
        animation: fade-in 1.5s ease-out 1.5s forwards;
    }

    .animate-fade-in-L3 {
        animation: fade-in 1.5s ease-out 2s forwards;
    }
</style>
