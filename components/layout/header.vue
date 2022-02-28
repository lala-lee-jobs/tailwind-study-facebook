<template>
  <header class="flex items-center justify-between px-4">
    <!-- header left -->
    <div class="flex items-center">
      <!-- FB logo -->
      <svg-icon name="logo" class="h-[39px] w-[39px] bg-fb rounded-full"/>
      <!-- Search Icon (只在小版顯示)-->
      <button class="popover-btn lg:hidden">
        <svg-icon name="search"/>
      </button>
      <!-- Search Bar (只在大版顯示)-->
      <div class="bg-fb-input ml-2 py-2 px-3 w-[240px] rounded-full flex-shrink items-center hidden lg:flex">
        <svg-icon name="search" class="w-[18px] h-[18px] mr-2"/>
        <input type="text" class="w-full bg-transparent text-white focus:outline-none" placeholder="搜尋 Facebook">
      </div>
    </div>
    <!-- header right -->
    <div class="flex items-center relative">
      <button class="popover-btn">
        <svg-icon name="plus"/>
      </button>
      <button class="popover-btn">
        <svg-icon name="messenger"/>
      </button>
      <button class="popover-btn">
        <svg-icon name="bell"/>
      </button>
      <button class="popover-btn">
        <svg-icon name="down"/>
      </button>
      <!-- 下拉選單 1 plus -->
      <div class="popover-panel">
        <p class="text-white mb-3 text-2xl">建立</p>
        <div class="flex items-center p-1 mb-2 hover:bg-fb-input rounded-lg cursor-pointer">
          <div class="bg-fb-input rounded-full p-2 mr-2 flex justify-center items-center">
            <svg-icon name="edit" class="w-[12px] h-[12px]"/>
          </div>
          <div class="flex-1">
            <p class="text-sm text-white mb-[2px]">貼文</p>
            <p class="text-xs text-gray-400">在動態消息分享貼文。</p>
          </div>
        </div>
      </div>
      <!-- 下拉選單 2 messenger -->
      <div class="popover-panel">
        <p class="text-white mb-3 text-2xl">Messenger</p>
        <div class="bg-fb-input rounded-full py-1 px-3 flex items-center mb-4">
          <svg-icon name="search" class="w-[18px] h-[18px] mr-2"/>
          <input type="text" class="w-full bg-transparent focus:outline-none text-white" placeholder="搜尋 Messenger">
        </div>
        <div class="flex items-center p-2 mb-2 hover:bg-fb-input rounded-lg cursor-pointer">
          <div class="w-[50px] h-[50px] rounded-full overflow-hidden mr-3">
            <img class="w-full object-cover" src="https://bruce-fe-fb.web.app/image/avator.png" alt="">
          </div>
          <div class="flex-1">
            <p class="text-base text-white mb-[2px]">布魯斯</p>
            <p class="text-sm text-gray-400">TailwindCSS讚讚！・1分鐘前</p>
          </div>
        </div>
      </div>
      <!-- 下拉選單 3 notification -->
      <div class="popover-panel">
        <p class="text-white mb-3 text-2xl">通知</p>
        <div class="flex items-center p-2 mb-2 hover:bg-fb-input rounded-lg cursor-pointer">
          <div class="w-[50px] h-[50px] rounded-full overflow-hidden mr-3">
            <img class="w-full object-cover" src="https://bruce-fe-fb.web.app/image/avator.png" alt="">
          </div>
          <div class="flex-1">
            <p class="text-sm text-white mb-[2px]">布魯斯發佈了一門新課程！</p>
            <p class="text-xs text-fb">1分鐘前</p>
          </div>
        </div>
      </div>
      <!-- 下拉選單 4 more -->
      <div class="popover-panel">
        <div class="flex items-center p-2 mb-2 hover:bg-fb-input rounded-lg cursor-pointer">
          <div class="w-[50px] h-[50px] rounded-full overflow-hidden mr-3">
            <img class="w-full object-cover" src="https://bruce-fe-fb.web.app/image/avator.png" alt="">
          </div>
          <div class="flex-1">
            <p class="text-base text-white mb-[2px]">布魯斯</p>
            <p class="text-sm text-gray-400">查看你的個人檔案</p>
          </div>
        </div>
        <div class="flex p-1 mb-2 items-center hover:bg-fb-input rounded-lg cursor-pointer">
          <div class="bg-fb-input rounded-full p-2 mr-2 flex justify-center items-center">
            <svg-icon name="logout" class="w-[22px] h-[22px]"/>
          </div>
          <p class="flex-1 text-white">登出</p>
        </div>
      </div>
    </div>
  </header>
</template>

<script>
  export default {
    name: 'LayoutHeader',
  };
</script>

<style></style>
