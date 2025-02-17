<template>
  <div>
    <!-- 首頁區塊 -->
    <div
      id="home"
      class="h-screen bg-gradient-to-b from-[#DADCF9] to-[#EFEFEB] flex flex-col justify-center items-center"
    >
      <h1 class="text-4xl font-bold mb-4">歡迎來到我們的網站</h1>
      <p class="text-xl text-gray-600 mb-8">提供專業的服務與優質的體驗</p>
      <button
        class="bg-blue-500 text-white px-6 py-2 rounded-lg hover:bg-blue-600"
      >
        了解更多
      </button>
    </div>

    <!-- 服務區塊 -->
    <div id="service" class="h-screen bg-white py-16">
      <div class="max-w-6xl mx-auto px-4">
        <h2 class="text-3xl font-bold mb-8 text-center">我們的服務</h2>
        <div class="grid grid-cols-3 gap-8">
          <div class="p-6 bg-gray-50 rounded-lg">
            <h3 class="text-xl font-semibold mb-4">服務項目一</h3>
            <p class="text-gray-600">
              提供全方位的解決方案，滿足您的各種需求。
            </p>
          </div>
          <div class="p-6 bg-gray-50 rounded-lg">
            <h3 class="text-xl font-semibold mb-4">服務項目二</h3>
            <p class="text-gray-600">專業團隊為您量身打造最適合的服務內容。</p>
          </div>
          <div class="p-6 bg-gray-50 rounded-lg">
            <h3 class="text-xl font-semibold mb-4">服務項目三</h3>
            <p class="text-gray-600">創新的技術支援，幫助您快速達成目標。</p>
          </div>
        </div>
      </div>
    </div>

    <!-- 關於我們區塊 -->
    <div id="about" class="h-screen bg-gray-100 py-16">
      <div class="max-w-4xl mx-auto px-4">
        <h2 class="text-3xl font-bold mb-8 text-center">關於我們</h2>
        <div class="bg-white p-8 rounded-lg shadow-lg">
          <p class="text-gray-600 mb-6">
            我們是一家專注於提供高品質服務的公司，擁有多年的行業經驗和專業團隊。
          </p>
          <p class="text-gray-600 mb-6">
            成立至今，我們已經服務超過數百位客戶，致力於為每一位客戶提供最好的解決方案。
          </p>
          <div class="grid grid-cols-3 gap-4 mt-8">
            <div class="text-center">
              <h4 class="text-2xl font-bold text-blue-500">500+</h4>
              <p class="text-gray-600">服務客戶</p>
            </div>
            <div class="text-center">
              <h4 class="text-2xl font-bold text-blue-500">10+</h4>
              <p class="text-gray-600">年度經驗</p>
            </div>
            <div class="text-center">
              <h4 class="text-2xl font-bold text-blue-500">100%</h4>
              <p class="text-gray-600">客戶滿意度</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
/* 如果需要添加自定義樣式可以在這裡補充 */
</style>
