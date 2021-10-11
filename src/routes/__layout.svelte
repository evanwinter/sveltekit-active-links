<script>
  import NavLink from "$lib/components/NavLink.svelte"
</script>

<div class="layout">
  <nav>
    <NavLink href="/">Home</NavLink>
    <NavLink href="/about">About</NavLink>
  </nav>

  <slot />
</div>

<style>
  .layout {
    max-width: 64rem;
    margin: 1rem auto;
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Oxygen,
      Ubuntu, Cantarell, "Open Sans", "Helvetica Neue", sans-serif;
  }

  nav {
    margin-bottom: 2rem;
  }
</style>
