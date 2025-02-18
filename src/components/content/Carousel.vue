<template>
  <div class="w-full max-w-5xl mx-auto px-4">
    <Carousel :items-to-show="1" :wrap-around="true" :autoplay="5000">
      <Slide v-for="slide in slides" :key="slide.id">
        <div class="p-1">
          <div class="relative overflow-hidden rounded-lg">
            <div class="aspect-[16/9]">
              <!-- 使用 16:9 比例 -->
              <img
                :src="slide.image"
                :alt="slide.title"
                class="w-full h-96 object-contain"
              />
            </div>
          </div>
        </div>
      </Slide>

      <template #addons>
        <Navigation />
        <Pagination />
      </template>
    </Carousel>
  </div>
</template>

<script setup>
import { Carousel, Slide, Pagination, Navigation } from 'vue3-carousel';
import 'vue3-carousel/dist/carousel.css';

const baseUrl = process.env.NODE_ENV === 'production' ? '/3c/' : '';

const slides = [
  {
    id: 1,
    image: `${baseUrl}/phone1.jpg`,
  },
  {
    id: 2,
    image: `${baseUrl}/phone2.jpg`,
  },
  {
    id: 3,
    image: `${baseUrl}/phone3.jpg`,
  },
];
</script>
