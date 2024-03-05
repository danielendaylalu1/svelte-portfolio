<script lang="ts">
  const navLinks: string[] = ["Home", "Aboutme", "Showcase"];
</script>

<ul class="nav">
  {#each navLinks as link (link)}
    <li class="nav-item">
      <a href={`#${link}`} class="nav-link">{link}</a>
    </li>
  {/each}
</ul>
