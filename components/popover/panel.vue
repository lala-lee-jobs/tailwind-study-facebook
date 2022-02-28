<template>
  <transition
    name="fade"
    mode="out-in"
    enter-active-class="duration-300 opacity-100"
    leave-active-class="duration-300 opacity-100"
    enter-class="translate-y-[10px] opacity-0"
    leave-to-class="translate-y-[10px] opacity-0"
  >
    <component :is="id"></component>
  </transition>
</template>
<script>
  // https://cn.vuejs.org/v2/guide/transitions.html
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
<style scoped></style>
