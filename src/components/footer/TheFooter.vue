<template>
  <div id="contact" class="bg-gray-200">
    <div
      class="container mx-auto py-8 flex flex-col justify-center items-center"
    >
      <div
        class="w-20 h-20 sm:w-24 sm:h-24 md:w-28 md:h-28 lg:w-32 lg:h-32 flex-shrink-0"
      >
        <img
          src="../../../public/logo.png"
          alt="Logo"
          class="w-full h-full object-contain"
        />
      </div>
      <div class="flex flex-col md:flex-row items-center gap-4 mt-4">
        <ul class="flex gap-4">
          <li>七天鑑賞</li>
          <li>原廠保固</li>
        </ul>
        <div class="flex items-center gap-4">
          <span>聯絡我們</span>
          <a
            href="#"
            class="text-gray-700 hover:text-blue-600 transition-colors"
          >
            <font-awesome-icon :icon="['fab', 'square-facebook']" size="xl" />
          </a>
          <a
            href="#"
            class="text-gray-700 hover:text-pink-600 transition-colors"
          >
            <font-awesome-icon :icon="['fab', 'instagram']" size="xl" />
          </a>
        </div>
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

// 添加圖示到函式庫
library.add(faSquareFacebook, faInstagram);

export default {
  name: 'Footer',
  components: {
    FontAwesomeIcon,
  },
};
</script>
