<template>
  <!-- 限時動態(可scoll) -->
  <div class="relative">
    <div class="no-scrollbar flex overflow-x-auto">
      <!-- 建立限時動態的卡片 -->
      <div class="min-w-[120px] flex-1 cursor-pointer px-[4px]">
        <div class="flex h-full flex-col">
          <div class="h-full overflow-hidden">
            <img
              class="h-full w-full object-cover duration-500 hover:scale-105"
              src="https://bruce-fe-fb.web.app/image/avator.png"
              alt=""
            />
          </div>
          <div class="relative bg-fb-card px-2 pt-6 pb-2">
            <button
              class="focus:outline-none absolute -top-4 left-[calc(50%-16px)] flex h-[32px] w-[32px] items-center justify-center rounded-full bg-fb p-2 ring ring-fb-card"
            >
              <svg-icon name="plus" class="h-[15px] w-[15px]" />
            </button>
            <p class="w-full text-center text-white">建立限時動態</p>
          </div>
        </div>
      </div>
      <!-- 顯示限時動態的卡片 -->
      <story-item v-for="n in 5" :id="getId(n)" :key="getId(n)"></story-item>
    </div>
    <button
      class="popover-btn absolute -right-3 top-[calc(50%-22.5px)] z-30 h-[45px] w-[45px]"
    >
      <svg-icon name="right-arrow" class="h-[45px] w-[45px]" />
    </button>
  </div>
</template>

<script>
  import StoryItem from './story-item.vue';
  export default {
    name: 'StoryList',
    components: { StoryItem },
    computed: {
      getId() {
        return (n) => `story-item-${n}`;
      },
    },
  };
</script>

<style></style>
