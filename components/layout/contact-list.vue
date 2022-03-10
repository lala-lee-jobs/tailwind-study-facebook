<template>
  <div>
    <p class="mb-2 text-lg text-gray-400">聯絡人</p>
    <template v-for="n in 10">
      <div
        :key="`contact-item-${n}`"
        class="flex w-full cursor-pointer items-center justify-items-center rounded py-2 px-1 hover:bg-fb-input"
      >
        <div class="w-[45px]">
          <div class="relative w-[32px] cursor-pointer">
            <div class="overflow-hidden rounded-full">
              <img src="https://bruce-fe-fb.web.app/image/avator.png" alt="" />
            </div>
            <div
              class="absolute bottom-0 right-0 h-[8px] w-[8px] rounded-full bg-green-500 ring ring-gray-900"
            ></div>
          </div>
        </div>
        <p class="text-[.9rem] text-white">布魯斯</p>
      </div>
    </template>
  </div>
</template>

<script>
  export default {
    name: 'LayoutContactList',
  };
</script>

<style></style>
