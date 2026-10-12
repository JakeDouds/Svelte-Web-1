<script>
    import Card from "$lib/components/Card.svelte";
</script>

<svelte:head>
    <title>SvelteKit Components Demo</title>
    <meta name="description" content="A demonstration of reusable SvelteKit components and props" />
</svelte:head>

<main>
    <h2>Our Example Cards</h2>

    <Card
        title="Learning SvelteKite"
        description="Components let us reuse interface elements across our application."
    />

    <Card
        title="Understanding Props"
        description="Props allow us to customise each component with different data."
    />
</main>

<style>
    main {
        display: flex;
        flex-wrap: wrap;
        align-items: center;
        justify-content: center;
    }
</style>