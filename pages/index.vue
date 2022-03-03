<template>
  <!-- 動態牆 -->
  <div class="max-w[745px] mx-auto w-full px-4">
    <story-list></story-list>
    <posts-wall></posts-wall>
  </div>
</template>

<script>
  import StoryList from '~/components/story/story-list.vue';
  import PostsWall from '~/components/posts/posts-wall.vue';
  export default {
    name: 'IndexPage',
    components: { StoryList, PostsWall },
  };
</script>
