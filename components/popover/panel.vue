<template>
  <!-- <transition
    name="fade"
    mode="out-in"
    enter-active-class="duration-300 opacity-100"
    leave-active-class="duration-300 opacity-100"
    enter-class="translate-y-[3px] opacity-0"
    leave-to-class="translate-y-[3px] opacity-0"
  > -->
  <transition name="fade" mode="out-in">
    <component :is="id"></component>
  </transition>
</template>
<script>
  export default {
    name: 'PopoverPanel',
    props: {
      id: {
        type: String,
        default: '',
      },
    },
  };
</script>
<style scoped>
  .fade-enter-active,
  .fade-leave-active {
    opacity: 1;
    transition: all 0.3s;
  }
  .fade-enter,
  .fade-leave-to {
    transform: translateY(3px);
    opacity: 0;
  }
</style>
