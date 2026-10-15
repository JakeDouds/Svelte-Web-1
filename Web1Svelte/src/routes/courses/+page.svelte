
<script>
    import Card from "$lib/components/Card.svelte";

    const courses = [
        {
            slug: 'programming',
            title: 'programming fundamentals',
            description: 'Learn programming and problem solving'
        },
        
        {
            slug: 'databases',
            title: 'database systems',
            description: 'learn relational databases and SQL'
        }
    ];
</script>
<svelte:head>
    <title> Our Courses</title>
</svelte:head>

<main>
    <h1> Our Courses</h1>

    {#each courses as course}
        <a href= {`/courses/${course.slug}`}>
        <Card 
            title={course.title}
            description={course.description}
            />
        </a>  
    {/each}
</main>