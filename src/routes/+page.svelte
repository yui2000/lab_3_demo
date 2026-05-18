<script>
  import projects from "$lib/projects.json";
  import Project from "$lib/Project.svelte";
</script>

<!-- <nav>
            <a href="." class="current">Home</a>
            <a href="projects">Projects</a>
            <a href="contact">Contact</a>
            <a href="resume">CV</a>
</nav> -->

    <h1>Hirasawa Yui</h1>

    <img src="images/image.png" alt="Hirasawa Yui" width="200">

    <p>Welcome to my website!</p>

    <div class="home">
    {#each projects.slice(0, 3) as p}
    <Project data={p} />
    {/each}
    </div>