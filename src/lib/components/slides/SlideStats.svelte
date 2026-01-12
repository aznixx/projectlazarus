<script lang="ts">
    import { onMount } from "svelte";
    import GridBackground from "$lib/components/GridBackground.svelte";

    let chartCanvas: HTMLCanvasElement;

    onMount(() => {
        const globalChart = (window as any).Chart;
        if (!globalChart || !chartCanvas) return;

        const ctx = chartCanvas.getContext("2d");
        if (!ctx) return;

        const gradient = ctx.createLinearGradient(0, 0, 0, 1200);
        gradient.addColorStop(0, "rgba(0, 245, 255, 1)");
        gradient.addColorStop(1, "rgba(0, 245, 255, 0.05)");

        new globalChart(ctx, {
            type: "bar",
            data: {
                labels: ["2020", "2021", "2022", "2023", "2024"],
                datasets: [
                    {
                        label: "Gestolen ($ Miljoen)",
                        data: [300, 429, 1700, 660, 1340],
                        backgroundColor: gradient,
                        border: "none",
                        borderWidth: 6,
                        hoverBackgroundColor: "#00f5ff",
                    },
                ],
            },
            options: {
                responsive: true,
                maintainAspectRatio: false,
                plugins: {
                    legend: { display: false },
                    tooltip: {
                        backgroundColor: "rgba(8, 10, 15, 0.98)",
                        titleFont: {
                            family: "Space Grotesk",
                            size: 28,
                            weight: "bold",
                        },
                        bodyFont: { family: "Inter", size: 28 },
                        padding: 24,
                        cornerRadius: 20,
                        borderColor: "rgba(0, 245, 255, 0.5)",
                        borderWidth: 4,
                        callbacks: {
                            label: (context: any) =>
                                ` $${context.parsed.y} Miljoen`,
                        },
                    },
                },
                scales: {
                    y: {
                        grid: { color: "rgba(255, 255, 255, 0.1)" },
                        ticks: {
                            color: "rgba(255, 255, 255, 0.5)",
                            font: {
                                family: "Space Grotesk",
                                size: 28,
                                weight: "bold",
                            },
                            callback: (value: any) =>
                                "$" + (value / 1000).toFixed(1) + "B",
                        },
                    },
                    x: {
                        grid: { display: false },
                        ticks: {
                            color: "#f1f5f9",
                            font: {
                                family: "Space Grotesk",
                                size: 32,
                                weight: "bold",
                            },
                        },
                    },
                },
            },
        });
    });
</script>

<div class="slide-view relative w-full h-full overflow-hidden">
    <GridBackground />

    <div
        class="relative z-10 flex flex-col h-full p-8 md:p-16 lg:p-20 gap-8 lg:gap-12 w-full"
    >
        <!-- Header -->
        <div
            class="flex flex-col lg:flex-row justify-between items-center lg:items-start gap-12"
        >
            <div class="space-y-4 text-center lg:text-left">
                <div
                    class="flex items-center justify-center lg:justify-start gap-4"
                >
                    <span
                        class="w-4 h-4 bg-teal-glow rounded-full shadow-[0_0_20px_#00f5ff]"
                    ></span>
                    <span
                        class="text-lg font-mono text-teal-glow uppercase tracking-[0.8em] font-black italic"
                        >FINANCIEEL</span
                    >
                </div>
                <h2
                    class="text-[4rem] md:text-[6.5rem] lg:text-[9rem] font-black text-white font-space tracking-tighter leading-none italic"
                >
                    HET <span class="text-teal-glow">GELD</span>
                </h2>
                <p
                    class="text-lg md:text-2xl text-slate-intel leading-tight max-w-5xl"
                >
                    Lazarus steelt miljarden voor <span
                        class="text-white font-bold italic">wapens</span
                    >.
                </p>
            </div>

            <div
                class="glass-panel-premium p-8 lg:p-12 rounded-[3rem] intel-border w-full lg:w-[600px] bg-crimson-glow/[0.04] shadow-[0_50px_100px_rgba(255,0,60,0.1)]"
            >
                <div class="flex items-center gap-6 mb-6">
                    <div
                        class="w-16 h-16 bg-crimson-glow/20 rounded-2xl flex items-center justify-center text-crimson-glow"
                    >
                        <i class="fas fa-biohazard text-3xl"></i>
                    </div>
                    <p
                        class="text-white font-black font-space text-lg md:text-xl tracking-widest uppercase italic"
                    >
                        GEVAAR
                    </p>
                </div>
                <p class="text-lg md:text-xl text-slate-intel leading-relaxed">
                    Experts in <span class="text-teal-glow italic font-bold"
                        >Bitcoin</span
                    >
                    en het
                    <span class="text-teal-glow italic font-bold"
                        >witwassen</span
                    >.
                </p>
            </div>
        </div>

        <!-- content Row: Filling the bottom area -->
        <div class="flex-1 flex flex-col xl:flex-row gap-12 lg:gap-24 min-h-0">
            <!-- Metrics Column -->
            <div class="xl:w-2/5 flex flex-col sm:flex-row xl:flex-col gap-8">
                <div
                    class="glass-panel-premium p-8 lg:p-10 rounded-[2.5rem] flex-1 flex flex-col justify-center border-t-4 border-white/5 group hover:intel-border transition-all duration-700"
                >
                    <p
                        class="text-slate-intel font-mono text-lg uppercase tracking-[0.4em] mb-4 font-black"
                    >
                        TOTAAL
                    </p>
                    <p
                        class="text-4xl md:text-6xl lg:text-7xl font-black text-white font-space mb-3 group-hover:text-teal-glow transition-colors italic leading-none"
                    >
                        $4.43 MILJARD
                    </p>
                    <p
                        class="text-lg md:text-xl text-teal-glow font-mono tracking-tighter uppercase font-black italic"
                    >
                        GEVAARLIJK
                    </p>
                </div>
                <div
                    class="glass-panel-premium p-8 lg:p-10 rounded-[2.5rem] flex-1 flex flex-col justify-center border-b-4 border-white/5"
                >
                    <p
                        class="text-slate-intel font-mono text-lg uppercase tracking-[0.4em] mb-4 font-black"
                    >
                        MARKTAANDEEL
                    </p>
                    <p
                        class="text-4xl md:text-6xl lg:text-7xl font-black text-white font-space mb-3 italic leading-none"
                    >
                        61%
                    </p>
                    <p
                        class="text-lg md:text-xl text-slate-intel font-mono tracking-tighter uppercase font-black italic"
                    >
                        MEERDERHEID
                    </p>
                </div>
            </div>

            <!-- Visualization Column: MASSIVE -->
            <div
                class="xl:w-3/5 glass-panel-premium rounded-[2.5rem] p-8 lg:p-10 border-2 border-white/5 flex flex-col h-[350px] lg:h-full relative overflow-hidden shadow-[0_60px_100px_rgba(0,0,0,0.8)]"
            >
                <div
                    class="absolute inset-0 bg-gradient-to-br from-teal-glow/[0.05] to-transparent"
                ></div>
                <div
                    class="flex justify-between items-center mb-16 relative z-10"
                >
                    <h4
                        class="text-slate-intel font-black font-space uppercase text-2xl lg:text-4xl tracking-[0.6em] flex items-center gap-10 italic"
                    >
                        <span class="w-24 h-2 bg-teal-glow/50 rounded-full"
                        ></span>
                        DOSSIER
                    </h4>
                    <span
                        class="text-xl text-slate-intel/40 font-mono tracking-[0.4em] font-black italic"
                        >MONITOR</span
                    >
                </div>
                <div class="flex-1 relative z-10">
                    <canvas bind:this={chartCanvas}></canvas>
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
