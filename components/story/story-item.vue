<template>
  <div
    :key="id"
    class="min-w-[120px] flex-1 cursor-pointer px-[4px]"
    @mouseover="hoverId = id"
    @mouseleave="hoverId = ''"
  >
    <div class="relative overflow-hidden">
      <div
        :class="{ hidden: hoverId === id }"
        class="absolute top-0 left-0 h-full w-full bg-black/20"
      ></div>
      <!-- 限動帳號頭像 -->
      <div
        class="absolute top-4 left-4 z-10 flex h-[32px] w-[32px] items-center justify-center rounded-full bg-fb-card ring-4 ring-fb"
      >
        <p class="text-sm text-white">布</p>
      </div>
      <!-- 漸層的遮罩 -->
      <div
        class="absolute top-0 left-0 z-20 h-full w-full bg-gradient-to-b from-black/30 to-transparent"
      ></div>
      <img
        :class="{ 'scale-105': hoverId === id }"
        class="h-full w-full duration-500 hover:scale-105"
        src="https://bruce-fe-fb.web.app/image/story.png"
        alt=""
      />
      <!-- 限動帳號名稱 -->
      <div class="absolute bottom-2 left-2 z-10 text-white">布魯斯</div>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'StoryItem',
    props: {
      id: {
        type: String,
        default: '',
      },
    },
    data() {
      return {
        hoverId: '',
      };
    },
  };
</script>

<style></style>
