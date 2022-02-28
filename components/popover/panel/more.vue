<template>
  <!-- 下拉選單 4 more -->
  <div class="popover-panel">
    <div
      class="mb-2 flex cursor-pointer items-center rounded-lg p-2 hover:bg-fb-input"
    >
      <div class="mr-3 h-[50px] w-[50px] overflow-hidden rounded-full">
        <img
          class="w-full object-cover"
          src="https://bruce-fe-fb.web.app/image/avator.png"
          alt=""
        />
      </div>
      <div class="flex-1">
        <p class="mb-[2px] text-base text-white">布魯斯</p>
        <p class="text-sm text-gray-400">查看你的個人檔案</p>
      </div>
    </div>
    <div
      class="mb-2 flex cursor-pointer items-center rounded-lg p-1 hover:bg-fb-input"
    >
      <div
        class="mr-2 flex items-center justify-center rounded-full bg-fb-input p-2"
      >
        <svg-icon name="logout" class="h-[22px] w-[22px]" />
      </div>
      <p class="flex-1 text-white">登出</p>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'PopoverPanelMore',
  };
</script>

<style></style>
