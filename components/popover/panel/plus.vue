<template>
  <!-- 下拉選單 1 plus -->
  <div class="popover-panel">
    <p class="mb-3 text-2xl text-white">建立</p>
    <div
      class="mb-2 flex cursor-pointer items-center rounded-lg p-1 hover:bg-fb-input"
    >
      <div
        class="mr-2 flex items-center justify-center rounded-full bg-fb-input p-2"
      >
        <svg-icon name="edit" class="h-[12px] w-[12px]" />
      </div>
      <div class="flex-1">
        <p class="mb-[2px] text-sm text-white">貼文</p>
        <p class="text-xs text-gray-400">在動態消息分享貼文。</p>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'PopoverPanelPlus',
  };
</script>

<style></style>
