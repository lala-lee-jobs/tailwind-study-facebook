<template>
  <div class="card px-0 pb-0">
    <!-- 貼文 (Loading) -->
    <div v-if="loading" class="animate-pulse">
      <!-- 貼文標題 -->
      <div class="mb-4 flex items-center px-4">
        <div
          class="mr-3 h-[44px] w-[44px] overflow-hidden rounded-full bg-fb-input"
        ></div>
        <div class="flex h-[50px] w-[200px] flex-wrap content-evenly">
          <div class="h-[16px] w-[200px] rounded-full bg-fb-input"></div>
          <div class="h-[12px] w-[100px] rounded-full bg-fb-input"></div>
        </div>
      </div>
      <!-- 貼文內容 -->
      <div class="h-[260px] w-full bg-fb-input"></div>
    </div>
    <!-- 貼文 (有內容) -->
    <div v-else>
      <post-header />
      <post-content />
    </div>
  </div>
</template>

<script>
  import PostContent from './post-content.vue';
  import PostHeader from './post-header.vue';
  export default {
    name: 'PostItem',
    components: { PostHeader, PostContent },
    props: {
      loading: {
        type: Boolean,
        default: false,
      },
    },
  };
</script>

<style></style>
