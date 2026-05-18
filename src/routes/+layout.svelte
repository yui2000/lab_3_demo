<script>
import { base } from "$app/paths";

    let pages = [
  {url: "/", title: "Home"},
  {url: "/projects", title: "Projects"},
  {url: "/resume", title: "Resume"},
  {url: "/contact", title: "Contact"},
  // add other pages here
];
</script>


<nav>
    {#each pages as p}
        <a href="{base}{p.url}">
            {p.title}
        </a>
    {/each}
</nav>

<slot />