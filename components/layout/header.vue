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
    <div class="flex items-center">
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
    </div>
  </header>
</template>

<script>
  export default {
    name: 'LayoutHeader',
  };
</script>

<style></style>
