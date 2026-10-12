<script>
    let {items = []} = $props();
</script>

<nav aria-label="Main navigation">

    <ul>
        {#each items as item}
        <li>
            <a href={item.href}>{item.label}</a>
        </li>
        {/each}
    </ul>
</nav>

<style>
    nav{
        border-top: 1px solid #ccc;
        margin-top: 1rem;
        padding-top: 1rem;
    }

    ul{
        display: flex;
        gap: 1.5rem;
        list-style: none;
        padding: center;
        margin: 0;
    }

    a{
        color: #3a2c00;
        text-decoration: none;
    }
    
    a:hover{
        text-decoration: underline;
    }
</style>