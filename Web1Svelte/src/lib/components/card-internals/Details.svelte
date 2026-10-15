<script>
    let {title = 'Example card', description = 'Card description goes here.'} = $props();
</script>

<div class="details">
    <h2>{title}</h2>
    <p>{description}</p>
</div>

<style>
    dl {
        display: grid;
        grid-template-columns: max-content 1fr;
        gap: 0.5rem 1rem;
    }
 
    dt {
        font-weight: bold;
    }
 
    dd {
        margin: 0;
    }
</style>