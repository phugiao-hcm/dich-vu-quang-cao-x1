<template>
  <section class="bg-white py-8 px-4">
    <div
      class="max-w-screen-xl mx-auto grid grid-cols-1 lg:grid-cols-2 gap-6 items-center"
    >
      <!-- Left Side -->
      <div class="flex flex-col items-start text-left gap-4">
        <!-- Clickable Image and Title -->
        <a
          href="#"
          class="w-full transform transition-transform duration-300 hover:scale-105 hover:shadow-lg"
        >
          <img src="/images/dichvu_1.png" alt="Hero Image" class="w-full" />
          <h2 class="text-3xl font-bold text-blue-600 mt-4">
            CHÀO SÂN RỰC LỬA<br />
            THỔI BÙNG SẮC RIÊNG
          </h2>
        </a>

        <!-- Promotion Buttons -->
        <div class="flex flex-wrap gap-4">
          <a
            href="#"
            class="bg-red-600 text-white px-4 py-2 rounded-full text-lg font-semibold transform transition-transform duration-300 hover:scale-105 hover:bg-red-700"
          >
            Áo Thun - 88K
          </a>
          <a
            href="#"
            class="bg-red-600 text-white px-4 py-2 rounded-full text-lg font-semibold transform transition-transform duration-300 hover:scale-105 hover:bg-red-700"
          >
            Túi Canvas - 29K
          </a>
        </div>
      </div>

      <!-- Right Side: Features -->
      <!-- Right Side: Features -->
      <!-- Right Side: Features -->
      <div class="grid grid-cols-2 gap-2">
        <!-- Box 1 -->
        <a
          href="#"
          class="bg-yellow-300 p-2 rounded-lg text-center w-full transform transition-transform duration-300 hover:scale-105 hover:shadow-lg"
        >
          <img
            src="/images/dichvu_2.png"
            alt="Online Order"
            class="w-full object-contain mb-2"
          />
          <p class="font-bold">ĐẶT HÀNG ONLINE</p>
          <p>Giảm ngay 10%</p>
        </a>

        <!-- Box 2 -->
        <a
          href="#"
          class="bg-green-600 p-2 rounded-lg text-white text-center w-full transform transition-transform duration-300 hover:scale-105 hover:shadow-lg"
        >
          <img
            src="/images/dichvu_3.png"
            alt="Free Delivery"
            class="w-full object-contain mb-2"
          />
          <p class="font-bold">GIAO HÀNG MIỄN PHÍ</p>
        </a>

        <!-- Box 3 -->
        <a
          href="#"
          class="bg-green-700 p-2 rounded-lg text-white text-center w-full transform transition-transform duration-300 hover:scale-105 hover:shadow-lg"
        >
          <img
            src="/images/dichvu_4.png"
            alt="Combo"
            class="w-full object-contain mb-2"
          />
          <p class="font-bold">ĐẶT GÓI COMBO</p>
          <p>Tiện ích đổ xô</p>
        </a>

        <!-- Box 4 -->
        <a
          href="#"
          class="bg-yellow-200 p-2 rounded-lg text-center w-full transform transition-transform duration-300 hover:scale-105 hover:shadow-lg"
        >
          <img
            src="/images/dichvu_5.png"
            alt="Online Approval"
            class="w-full object-contain mb-2"
          />
          <p class="font-bold">DUYỆT MẪU ONLINE</p>
        </a>
      </div>
    </div>
  </section>
</template>

<script setup>
// Bạn có thể đặt các ảnh như /public/images/...
</script>

<style scoped>
/* Tuỳ chọn thêm hiệu ứng hoặc font đặc biệt */
</style>
