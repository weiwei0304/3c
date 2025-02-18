<template>
  <div class="fixed top-0 left-0 right-0 z-50 bg-red-100">
    <div class="px-4 py-0.5 relative">
      <div class="flex justify-between items-center">
        <!-- Logo 容器使用響應式尺寸 -->
        <div
          class="w-20 h-20 sm:w-24 sm:h-24 md:w-28 md:h-28 lg:w-32 lg:h-32 flex-shrink-0"
        >
          <img
            src="../../../public/logo.png"
            alt="Logo"
            class="w-full h-full object-contain"
          />
        </div>

        <!-- hamburger -->
        <button class="md:hidden" @click="toggleMenu">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            fill="none"
            viewBox="0 0 24 24"
            stroke="currentColor"
            class="w-6 h-6"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M4 6h16M4 12h16M4 18h16"
            />
          </svg>
        </button>
        <nav
          class="absolute md:relative left-0 right-0 top-[84px] sm:top-[100px] md:top-0 w-full md:w-auto"
        >
          <ul
            class="bg-white md:bg-transparent flex flex-col md:flex-row md:space-x-6 transition-all duration-300 ease-out md:transition-none overflow-hidden w-full md:w-auto shadow-lg md:shadow-none"
            :class="{
              'max-h-[300px] opacity-100 translate-y-0': isMenuOpen,
              'max-h-0 opacity-0 -translate-y-4': !isMenuOpen,
              'md:max-h-none md:opacity-100 md:translate-y-0': true,
            }"
          >
            <li
              class="border-b md:border-none p-4 md:p-0 hover:bg-gray-100 md:hover:bg-transparent"
            >
              <a
                href="#"
                @click.prevent="scrollToSection('service')"
                class="block w-full text-gray-700 hover:text-gray-900"
              >
                服務項目
              </a>
            </li>
            <li
              class="border-b md:border-none p-4 md:p-0 hover:bg-gray-100 md:hover:bg-transparent"
            >
              <a
                href="#"
                @click.prevent="scrollToSection('about')"
                class="block w-full text-gray-700 hover:text-gray-900"
              >
                關於我們
              </a>
            </li>
            <li
              class="border-b md:border-none p-4 md:p-0 hover:bg-gray-100 md:hover:bg-transparent"
            >
              <a
                href="#"
                @click.prevent="scrollToSection('contact')"
                class="block w-full text-gray-700 hover:text-gray-900"
              >
                聯絡我們
              </a>
            </li>
          </ul>
        </nav>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      isMenuOpen: false,
    };
  },
  methods: {
    scrollToSection(sectionId) {
      const element = document.getElementById(sectionId);
      if (element) {
        element.scrollIntoView({ behavior: 'smooth' });
      }
      this.isMenuOpen = false;
    },
    toggleMenu() {
      this.isMenuOpen = !this.isMenuOpen;
    },
  },
};
</script>
