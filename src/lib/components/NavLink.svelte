<script>
  import { page } from "$app/stores"
  $: isActive = $page.path === $$props.href
</script>

<a {...$$props} class:active={isActive}>
  <slot />
</a>

<style>
  a {
    color: black;
    text-decoration: none;
    padding: 1rem;
  }
  a.active {
    background: lightgray;
  }
</style>
