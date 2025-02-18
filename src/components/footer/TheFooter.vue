<template>
  <div id="contact" class="bg-gray-100">
    <div class="container mx-auto py-12 px-4">
      <!-- 主要內容區域 -->
      <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
        <!-- Logo 和簡介區塊 -->
        <div class="flex flex-col items-center md:items-start">
          <div class="w-24 h-24 mb-4">
            <img
              src="../../../public/logo.png"
              alt="Logo"
              class="w-full h-full object-contain"
            />
          </div>
        </div>

        <!-- 聯絡資訊和社群媒體組合區塊 -->
        <div class="flex flex-col items-center md:items-start space-y-8">
          <!-- 聯絡資訊區塊 -->
          <!-- 聯絡資訊區塊 -->
          <div class="flex flex-col space-y-4">
            <h3 class="text-lg font-semibold text-gray-800 mb-2">聯絡資訊</h3>
            <div class="flex flex-col space-y-3 text-gray-600">
              <!-- 地址 -->
              <a
                href="https://maps.google.com/?q=台北市松山區民生東路三段113巷25弄33號"
                target="_blank"
                rel="noopener noreferrer"
                class="flex items-center group transition-colors"
                aria-label="在地圖上查看我們的位置"
                title="點擊查看地圖"
              >
                <font-awesome-icon
                  :icon="['fas', 'location-dot']"
                  class="w-5 mr-3 text-gray-500 group-hover:text-blue-600 transition-colors"
                />
                <span class="group-hover:text-blue-600 transition-colors">
                  台北市松山區民生東路三段113巷25弄33號
                </span>
              </a>

              <!-- 電話 -->
              <a
                href="tel:0906038198"
                class="flex items-center group transition-colors"
                aria-label="撥打電話給我們"
                title="點擊撥打電話"
              >
                <font-awesome-icon
                  :icon="['fas', 'phone']"
                  class="w-5 mr-3 text-gray-500 group-hover:text-blue-600 transition-colors"
                />
                <span class="group-hover:text-blue-600 transition-colors">
                  0906-038-198
                </span>
              </a>

              <!-- 營業時間 -->
              <div class="flex items-center">
                <font-awesome-icon
                  :icon="['fas', 'clock']"
                  class="w-5 mr-3 text-gray-500"
                />
                <span>週一至週六 12:30-21:00</span>
              </div>
            </div>
          </div>

          <!-- 社群媒體區塊 -->
          <div class="flex flex-col space-y-4">
            <h3 class="text-lg font-semibold text-gray-800 mb-2">關注我們</h3>
            <div class="flex gap-4">
              <a
                href="https://m.facebook.com/100064015510294/"
                class="bg-gray-200 hover:bg-blue-100 p-3 rounded-xl transition-colors"
              >
                <font-awesome-icon
                  :icon="['fab', 'square-facebook']"
                  class="text-blue-600 text-2xl"
                />
              </a>

              <a
                href="https://www.instagram.com/chaoyu_3c/"
                class="bg-gray-200 hover:bg-pink-100 p-3 rounded-xl transition-colors"
              >
                <font-awesome-icon
                  :icon="['fab', 'instagram']"
                  class="text-pink-600 text-2xl"
                />
              </a>
            </div>
          </div>
        </div>
      </div>

      <!-- 版權信息 -->
      <div
        class="mt-12 pt-4 border-t border-gray-200 text-center text-gray-500 text-sm"
      >
        <p>
          &copy; {{ new Date().getFullYear() }} 潮宇3C空間. All rights reserved.
        </p>
      </div>
    </div>
  </div>
</template>

<script>
import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome';
import { library } from '@fortawesome/fontawesome-svg-core';
import {
  faSquareFacebook,
  faInstagram,
} from '@fortawesome/free-brands-svg-icons';
import {
  faLocationDot,
  faPhone,
  faClock,
  faCheckCircle,
  faShieldAlt,
} from '@fortawesome/free-solid-svg-icons';

library.add(
  faSquareFacebook,
  faInstagram,
  faLocationDot,
  faPhone,
  faClock,
  faCheckCircle,
  faShieldAlt
);

export default {
  name: 'Footer',
  components: {
    FontAwesomeIcon,
  },
};
</script>

<style scoped></style>
