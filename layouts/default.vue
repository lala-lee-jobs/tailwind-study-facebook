<template>
  <div>
    <layout-header
      class="fixed top-0 left-0 right-0 z-50 h-[56px] w-full bg-fb-header"
    />
    <main class="z-0 flex min-h-[100vh] pt-main-span">
      <layout-menu-list
        class="sticky top-main-span hidden h-full w-full max-w-[360px] pl-4 lg:block"
      />
      <nuxt class="mx-auto h-[200vh] w-full max-w-[744px]" />
      <layout-contact-list
        class="sticky top-main-span hidden h-full w-full max-w-[360px] lg:block"
      />
    </main>
  </div>
</template>

<script>
  export default {
    name: 'LayoutDefault',
  };
</script>

<style></style>
