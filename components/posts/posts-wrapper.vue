<template>
  <div>
    <post-item />
    <template v-for="n in 5">
      <post-item :key="`post-item-loading-${n}`" loading />
    </template>
  </div>
</template>

<script>
  import PostItem from './post-item.vue';
  export default {
    name: 'PostsWrapper',
    components: { PostItem },
  };
</script>

<style></style>
