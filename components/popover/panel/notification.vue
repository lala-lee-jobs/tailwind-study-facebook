<template>
  <!-- 下拉選單 3 notification -->
  <div class="popover-panel">
    <p class="mb-3 text-2xl text-white">通知</p>
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
        <p class="mb-[2px] text-sm text-white">布魯斯發佈了一門新課程！</p>
        <p class="text-xs text-fb">1分鐘前</p>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'PopoverPanelNotification',
  };
</script>

<style></style>
