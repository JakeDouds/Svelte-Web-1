<script>
    let {course='ID512 Web Development', year=2026} = $props();
</script>

<footer>    
    <p>{course} &copy; {year}</p>
</footer>

<style>
    footer {
        background-color: #fda053;
        padding: 1rem;
        border-top: 1px solid #991f00;
        text-align: center;
        margin-bottom: 1rem;
    }
</style>