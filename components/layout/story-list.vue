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
      <template v-for="n in 5">
        <div
          :id="getId(n)"
          :key="getId(n)"
          class="min-w-[120px] flex-1 cursor-pointer px-[4px]"
          @mouseover="hoverId = getId(n)"
          @mouseleave="hoverId = ''"
        >
          <div class="relative overflow-hidden">
            <div
              :class="{ hidden: hoverId === getId(n) }"
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
              :class="{ 'scale-105': hoverId === getId(n) }"
              class="h-full w-full duration-500 hover:scale-105"
              src="https://bruce-fe-fb.web.app/image/story.png"
              alt=""
            />
            <!-- 限動帳號名稱 -->
            <div class="absolute bottom-2 left-2 z-10 text-white">布魯斯</div>
          </div>
        </div>
      </template>
    </div>
    <button
      class="popover-btn absolute -right-3 top-[calc(50%-22.5px)] z-10 h-[45px] w-[45px]"
    >
      <svg-icon name="right-arrow" class="h-[45px] w-[45px]" />
    </button>
  </div>
</template>

<script>
  export default {
    name: 'StoryList',
    data() {
      return {
        hoverId: '',
      };
    },
    computed: {
      getId() {
        return (n) => `story-item-${n}`;
      },
    },
  };
</script>

<style></style>
