<template>
  <div>
    <!-- 文字 Post 建立 -->
    <div class="flex pb-4">
      <div class="mr-3 w-[40px] overflow-hidden rounded-full">
        <img src="https://bruce-fe-fb.web.app/image/avator.png" alt="" />
      </div>
      <div class="flex flex-1 items-center rounded-full bg-fb-input">
        <p class="pl-3 text-left text-sm text-gray-400">布魯斯，在想些什麼？</p>
      </div>
    </div>
    <!-- 多媒體 Post 建立 -->
    <div class="flex border-t border-gray-700 pt-3">
      <button
        v-for="(item, index) in richPostButtons"
        :key="`rich-post-button-${index}`"
        class="flex h-[40px] flex-1 items-center justify-center rounded-lg hover:bg-fb-input"
      >
        <div class="w-[16px]">
          <img :src="item.url" alt="" />
        </div>
        <p class="pl-1.5 text-sm text-gray-400">{{ item.text }}</p>
      </button>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'CreatePost',
    computed: {
      richPostButtons() {
        return [
          {
            url: 'https://bruce-fe-fb.web.app/image/camera.svg',
            text: '直播視訊',
          },
          {
            url: 'https://bruce-fe-fb.web.app/image/photo.svg',
            text: '相片/影片',
          },
          {
            url: 'https://bruce-fe-fb.web.app/image/feel.svg',
            text: '感受/活動',
          },
        ];
      },
    },
  };
</script>

<style></style>
