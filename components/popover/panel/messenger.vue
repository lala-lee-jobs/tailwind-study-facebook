<template>
  <!-- 下拉選單 2 messenger -->
  <div class="popover-panel">
    <p class="mb-3 text-2xl text-white">Messenger</p>
    <div class="mb-4 flex items-center rounded-full bg-fb-input py-1 px-3">
      <svg-icon name="search" class="mr-2 h-[18px] w-[18px]" />
      <input
        type="text"
        class="focus:outline-none w-full bg-transparent text-white"
        placeholder="搜尋 Messenger"
      />
    </div>
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
        <p class="text-sm text-gray-400">TailwindCSS讚讚！・1分鐘前</p>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'PopoverPanelMessenger',
  };
</script>

<style></style>
