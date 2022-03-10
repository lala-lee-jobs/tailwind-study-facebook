<template>
  <div
    class="mb-1 flex w-full cursor-pointer items-center justify-items-center rounded p-2 hover:bg-fb-input"
  >
    <div class="mr-4 w-[32px] overflow-hidden rounded-full">
      <img class="w-full object-cover" :src="url" alt="" />
    </div>
    <div class="text-[.9rem] text-white">
      {{ text }}
    </div>
  </div>
</template>

<script>
  export default {
    name: 'InfoItem',
    props: {
      url: {
        type: String,
        default: '',
      },
      text: {
        type: String,
        default: '',
      },
    },
  };
</script>

<style></style>
