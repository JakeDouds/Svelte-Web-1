<script>
    import Navigation from './Nav.svelte';
    let {title = 'Sveltekit Component',
        subtitle = 'For more info see the sveltekit tutorial',
        navItems = []
    } = $props();
</script>

<header>
    <h1> {title}</h1>
    <p> {subtitle}</p>
    <Navigation items = {navItems} />
</header>

<style>
    header {
        background-color: #fda053;
        padding: 1rem;
        border-bottom: 1px solid #991f00;
        text-align: center;
    }
</style>