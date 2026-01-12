<script lang="ts">
    import SlideTitle from "$lib/components/slides/SlideTitle.svelte";
    import SlideIntro from "$lib/components/slides/SlideIntro.svelte";
    import SlideProfile from "$lib/components/slides/SlideProfile.svelte";
    import SlideTimeline from "$lib/components/slides/SlideTimeline.svelte";
    import SlideKillChain from "$lib/components/slides/SlideKillChain.svelte";
    import SlideStats from "$lib/components/slides/SlideStats.svelte";
    import SlideImpact from "$lib/components/slides/SlideImpact.svelte";
    import SlideConclusion from "$lib/components/slides/SlideConclusion.svelte";

    const components = [
        SlideTitle,
        SlideIntro,
        SlideProfile,
        SlideTimeline,
        SlideKillChain,
        SlideStats,
        SlideImpact,
        SlideConclusion,
    ];
</script>

<div class="bg-[#020205] min-h-screen">
    {#each components as Slide, i}
        <div class="slide-page">
            <svelte:component this={Slide} />
        </div>
    {/each}
</div>

<style>
    .slide-page {
        width: 1280px;
        height: 720px;
        margin: 0 auto;
        position: relative;
        overflow: hidden;
        page-break-after: always;
        break-after: page;
    }

    @media print {
        :global(body) {
            background-color: #0f172a !important;
            -webkit-print-color-adjust: exact;
            print-color-adjust: exact;
        }
        .slide-page {
            width: 100vw;
            height: 100vh;
        }
    }
</style>
