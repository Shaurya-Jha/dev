<script>
  // MDsveX passes all frontmatter keys down as exports
  let { title, children } = $props();
</script>

<main class="w-full">
  <!-- The prose class will now be recognized by Tailwind v4 -->
  <article class="prose mx-auto">
    <header class="mb-10">
      <h1>{title}</h1>
    </header>

    <!-- Render markdown directly into the prose container -->
    {@render children()}
  </article>
</main>