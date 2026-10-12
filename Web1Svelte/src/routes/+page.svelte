<script>
    import Card from "$lib/components/Card.svelte";
    import Footer from "$lib/components/Footer.svelte";
    import Header from "$lib/components/Header.svelte";

    const navigationLinks = [
        {label: 'Home', href: '/'},
        {label: 'About', href: '/about'},
        {label: 'Content', href: '/content'}
    ]
</script>

<svelte:head>
    <title>SvelteKit Components Demo</title>
    <meta name="description" content="A demonstration of reusable SvelteKit components and props" />
</svelte:head>

<Header
    navItems={navigationLinks}
/>
<main>
    <h2>Our Example Card</h2>

    <Card
        title="Learning SvelteKite"
        description="Components let us reuse interface elements across our application."
    />

    <Card
        title="Understanding Props"
        description="Props allow us to customise each component with different data."
    />
</main>

<Footer course="ID512 Web Development" year={2026} />

<style>
    main {
        display: flex;
        flex-wrap: wrap;
        align-items: center;
        justify-content: center;
    }
</style>