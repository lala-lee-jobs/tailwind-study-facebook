<template>
  <div>
    <layout-header />
    <main class="flex min-h-[100vh] pt-main-span">
      <layout-menu-list />
      <nuxt />
      <layout-contact-list />
    </main>
  </div>
</template>

<script>
  export default {
    name: 'LayoutDefault',
  };
</script>

<style></style>
