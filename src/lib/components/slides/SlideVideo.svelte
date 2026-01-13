<script>
    import GridBackground from "$lib/components/GridBackground.svelte";
</script>

<div class="slide-view relative w-full h-full overflow-hidden">
    <GridBackground />

    <div
        class="relative z-10 flex flex-col h-full p-8 md:p-16 lg:p-20 items-center justify-center gap-8 md:gap-12"
    >
        <!-- Header -->
        <div class="text-center space-y-4">
            <h2
                class="text-[3rem] md:text-[5rem] lg:text-[7rem] font-black text-white font-space tracking-tighter leading-none italic"
            >
                SPEAR <span class="text-crimson-glow">PHISHING</span>
            </h2>
            <p
                class="text-slate-intel font-mono text-sm md:text-lg tracking-widest uppercase"
            >
                // VIDEO BRIEFING (02:00)
            </p>
        </div>

        <!-- Video Container -->
        <div class="relative w-full max-w-5xl aspect-video group">
            <!-- Glow Effect -->
            <div
                class="absolute -inset-1 bg-gradient-to-r from-crimson-glow via-purple-500 to-blue-600 rounded-2xl opacity-50 blur-xl group-hover:opacity-75 transition-opacity duration-700"
            ></div>

            <!-- Glass Border -->
            <div
                class="relative h-full w-full rounded-2xl p-1 bg-gradient-to-br from-white/20 to-white/5 backdrop-blur-sm border border-white/10"
            >
                <!-- Video Placeholder / Content -->
                <div
                    class="w-full h-full bg-black/80 rounded-xl overflow-hidden flex items-center justify-center relative"
                >
                    <!-- Replace 'src' with your actual video or use an iframe for YouTube/Vimeo -->
                    <iframe
                        class="w-full h-full"
                        src="https://www.youtube.com/embed/7zNbcWuZRzg?si=j0U2lOSdf6S2gHH2"
                        frameborder="0"
                        allowfullscreen
                    ></iframe>
                </div>
            </div>

            <!-- Decorative elements -->
            <div
                class="absolute -bottom-12 -right-12 text-crimson-glow/20 text-9xl font-black font-space italic select-none pointer-events-none z-0"
            >
                REC
            </div>
        </div>
    </div>
</div>

<style>
    .slide-view {
        background-color: #020205;
    }
</style>
