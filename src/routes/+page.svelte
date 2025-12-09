<script lang="ts">
    import Header from "$lib/components/Header.svelte";
    import Hero from "$lib/components/Hero.svelte";
    import Logos from "$lib/components/Logos.svelte";
    import Problem from "$lib/components/Problem.svelte";
    import Solution from "$lib/components/Solution.svelte";
    import Footer from "$lib/components/Footer.svelte";
</script>

<main class="min-h-screen bg-[#050505] text-white selection:bg-[var(--color-primary)] selection:text-white">
    <Header />
    <Hero />
    <Logos />
    <Problem />
    <Solution />
    <Footer />
</main>

