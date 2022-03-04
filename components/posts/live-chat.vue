<template>
  <div>
    <div v-swiper:liveChatSwiper="swiperOptions" class="swiper-container">
      <div class="swiper-wrapper">
        <!-- 建立包廂 按鈕 -->
        <div class="swiper-slide">
          <button
            class="focus:outline-none mr-4 flex h-[40px] items-center rounded-full px-4 ring-2 ring-gray-600"
          >
            <div class="w-[24px]">
              <img src="https://bruce-fe-fb.web.app/image/video.svg" alt="" />
            </div>
            <div class="ml-2 text-sm font-bold text-fb">建立包廂</div>
          </button>
        </div>
        <!-- 正在直播包廂清單 -->
        <div v-for="n in 20" :key="`swiper-slide-${n}`" class="swiper-slide">
          <div class="w-[55px]">
            <div class="relative w-[40px] cursor-pointer">
              <div class="overflow-hidden rounded-full">
                <img
                  src="https://bruce-fe-fb.web.app/image/avator.png"
                  alt=""
                />
              </div>
              <div
                class="absolute bottom-0 right-0 h-[10px] w-[10px] rounded-full bg-green-500 ring ring-gray-900"
              ></div>
            </div>
          </div>
        </div>
      </div>
      <!-- Navigation Buttons absolute in swiper-container -->
      <div class="swiper-button-prev"></div>
      <div class="swiper-button-next"></div>
    </div>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        swiperOptions: {
          loop: false,
          slidesPerView: 'auto',
          navigation: {
            nextEl: '.swiper-button-next',
            prevEl: '.swiper-button-prev',
          },
        },
      };
    },
    mounted() {
      // console.log('Current Swiper instance object', this.liveChatSwiper);
    },
  };
</script>

<style></style>
