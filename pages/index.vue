<template>
  <!-- 動態牆 -->
  <div class="max-w[745px] mx-auto w-full px-4">
    <story-list></story-list>
  </div>
</template>

<script>
  import storyList from '~/components/layout/story-list.vue';
  export default {
    name: 'IndexPage',
    components: { storyList },
  };
</script>
