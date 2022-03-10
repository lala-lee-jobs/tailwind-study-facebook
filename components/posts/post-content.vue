<template>
  <div>
    <!-- 貼文內文 -->
    <p class="mt-3 px-4 text-base text-gray-300">
      【布魯斯】手作蛋糕高雄分店開幕囉！！
    </p>
    <!-- 貼文圖片 -->
    <a href="#" class="mt-3 block">
      <div class="h-[260px] w-full overflow-hidden">
        <img
          class="w-full object-cover"
          src="https://bruce-fe-fb.web.app/image/item.png"
          alt=""
        />
      </div>
      <div class="w-full bg-fb-input px-4 py-2 text-white">
        <div class="text-sm text-gray-400">WWW.BRUCEFE.COM</div>
        <div class="text-lg">【布魯斯】手作蛋糕高雄分店開幕囉！！</div>
      </div>
    </a>
    <!-- 讚、留言 -->
    <div class="px-4">
      <div class="flex justify-between border-b border-gray-700 py-3">
        <!-- 讚 -->
        <div class="flex items-center">
          <div class="mr-2 w-[18px]">
            <img src="https://bruce-fe-fb.web.app/image/like-blue.svg" alt="" />
          </div>
          <p class="text-sm text-gray-400">990</p>
        </div>
        <!-- 留言/分享 -->
        <div class="flex items-center">
          <div class="mr-2 text-sm text-gray-400">4則留言</div>
          <div class="text-sm text-gray-400">1次分享</div>
        </div>
      </div>
      <div class="flex items-center py-2">
        <button
          class="flex h-[40px] flex-1 items-center justify-center rounded-lg hover:bg-fb-input"
        >
          <div class="w-[16px]">
            <img src="https://bruce-fe-fb.web.app/image/like.svg" alt="" />
          </div>
          <div class="pl-1.5 text-sm text-gray-400">讚</div>
        </button>
        <button
          class="flex h-[40px] flex-1 items-center justify-center rounded-lg hover:bg-fb-input"
        >
          <div class="w-[16px]">
            <img src="https://bruce-fe-fb.web.app/image/chat.svg" alt="" />
          </div>
          <div class="pl-1.5 text-sm text-gray-400">留言</div>
        </button>
        <button
          class="flex h-[40px] flex-1 items-center justify-center rounded-lg hover:bg-fb-input"
        >
          <div class="w-[16px]">
            <img src="https://bruce-fe-fb.web.app/image/share.svg" alt="" />
          </div>
          <div class="pl-1.5 text-sm text-gray-400">分享</div>
        </button>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'PostContent',
  };
</script>

<style></style>
