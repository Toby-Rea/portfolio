<script lang="ts" setup>
  useHead({
    title: 'Toby Rea',
  })
</script>

<template>
  <div>
    <header>
      <nav class="flex items-center justify-center gap-6 py-6 bg-slate-100">
        <NuxtLink to="/">Home</NuxtLink>
        <NuxtLink to="/blog">Blog</NuxtLink>
        <NuxtLink to="/contact">Contact</NuxtLink>
      </nav>
    </header>

    <main>
      <slot />
    </main>
  </div>
</template>

<style scoped>
  body {
    margin: 0;
    padding: 0;
    display: flex;
    flex-direction: column;
    height: 100vh;
  }

  main {
    display: flex;
    flex-direction: column;
    place-items: center;
    height: 100%;
  }
</style>
