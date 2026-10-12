<script>
    import Picture from "./card-internals/Picture.svelte"
    import Details from "./card-internals/Details.svelte"
    let {title = 'Example Card', description='This is an example of a reusable component.'}=$props();
</script>

<article class="card">
    <Picture />
    <Details {title} {description} />
</article>

<style>
    .card{
        background-color: #ffc063;
        display: flex;
        align-items: center;
        gap: 2rem;
        border: 2px solid #b10808;
        border-radius: 25px;
        padding: 1rem;
        max-width: 600px;
        margin: 1rem;
        bottom: 100rem;
    }
</style>