<template>
  <header class="flex items-center justify-between px-4">
    <!-- header left -->
    <div class="flex items-center">
      <!-- FB logo -->
      <svg-icon name="logo" class="h-[39px] w-[39px] rounded-full bg-fb" />
      <!-- Search Icon (只在小版顯示)-->
      <button class="popover-btn lg:hidden">
        <svg-icon name="search" />
      </button>
      <!-- Search Bar (只在大版顯示)-->
      <div
        class="ml-2 hidden w-[240px] flex-shrink items-center rounded-full bg-fb-input py-2 px-3 lg:flex"
      >
        <svg-icon name="search" class="mr-2 h-[18px] w-[18px]" />
        <input
          type="text"
          class="focus:outline-none w-full bg-transparent text-white"
          placeholder="搜尋 Facebook"
        />
      </div>
    </div>
    <!-- header right -->
    <div class="relative flex items-center">
      <button
        class="popover-btn"
        @click.stop="popoverPanelId = 'popover-panel-plus'"
      >
        <svg-icon name="plus" />
      </button>
      <button
        class="popover-btn"
        @click.stop="popoverPanelId = 'popover-panel-messenger'"
      >
        <svg-icon name="messenger" />
      </button>
      <button
        class="popover-btn"
        @click.stop="popoverPanelId = 'popover-panel-notification'"
      >
        <svg-icon name="bell" />
      </button>
      <button
        class="popover-btn"
        @click.stop="popoverPanelId = 'popover-panel-more'"
      >
        <svg-icon name="down" />
      </button>
      <popover-panel
        :id="popoverPanelId"
        v-click-outside="clickOutsideHandler"
      />
    </div>
  </header>
</template>

<script>
  import vClickOutside from 'v-click-outside';
  export default {
    name: 'LayoutHeader',
    directives: {
      clickOutside: vClickOutside.directive,
    },
    data() {
      return {
        popoverPanelId: '',
      };
    },
    methods: {
      clickOutsideHandler(event) {
        this.popoverPanelId = '';
      },
    },
  };
</script>

<style></style>
