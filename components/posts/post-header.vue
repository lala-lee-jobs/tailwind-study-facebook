<template>
  <!-- 貼文標題 -->
  <div class="flex px-4">
    <div class="mr-3 w-[44px] overflow-hidden rounded-full">
      <img src="https://bruce-fe-fb.web.app/image/avator.png" alt="" />
    </div>
    <div class="flex-1">
      <p class="text-white">布魯斯前端</p>
      <div class="flex items-center text-sm text-gray-400">
        <div>5小時</div>
        <div>．</div>
        <div class="w-[12px]">
          <img
            class="w-full"
            src="https://bruce-fe-fb.web.app/image/earth.svg"
            alt=""
          />
        </div>
      </div>
    </div>
    <button class="focus:outline-none w-[12px]">
      <img src="https://bruce-fe-fb.web.app/image/more.svg" alt="" />
    </button>
  </div>
</template>

<script>
  export default {
    name: 'PostHeader',
  };
</script>

<style></style>
