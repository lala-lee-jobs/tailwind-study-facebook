<template>
  <div>
    <post-header />
    <post-content />
  </div>
</template>

<script>
  import PostContent from './post-content.vue';
  import PostHeader from './post-header.vue';
  export default {
    name: 'PostsWrapper',
    components: { PostHeader, PostContent },
  };
</script>

<style></style>
