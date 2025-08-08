<template>
  <section class="bg-white py-10 px-4">
    <div class="max-w-7xl mx-auto">
      <h2 class="text-2xl font-bold text-red-600 mb-6 uppercase">
        Danh mục sản phẩm
      </h2>
      <div
        class="grid grid-cols-2 sm:grid-cols-3 md:grid-cols-4 lg:grid-cols-6 gap-4"
      >
        <div
          v-for="(item, index) in categories"
          :key="index"
          class="border-2 border-red-500 rounded-lg p-4 flex flex-col items-center text-center hover:shadow-lg transition"
        >
          <img
            :src="item.image"
            :alt="item.name"
            class="h-20 mb-2 object-contain"
          />
          <p class="text-sm font-medium">{{ item.name }}</p>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
const categories = [
  { name: "Bìa Đựng Hồ", image: "images/category_1.png" },
  { name: "Danh Thiếp", image: "images/category_2.png" },
  { name: "Vé", image: "images/category_3.png" },
  { name: "Tờ Gấp", image: "images/category_4.png" },
  { name: "Poster", image: "images/category_5.png" },
  { name: "Hộp Giấy", image: "images/category_6.png" },
  { name: "Túi Giấy", image: "images/category_7.png" },
  { name: "Biểu Mẫu", image: "images/category_8.png" },
  { name: "Thẻ Nhựa", image: "images/category_9.png" },
  { name: "Thực Đơn", image: "images/category_10.png" },
  { name: "Giấy Tiêu Đề", image: "images/category_11.png" },
  { name: "Bao Thư", image: "images/category_12.png" },
  { name: "Tờ Rơi", image: "images/category_13.png" },
  { name: "Catalogue", image: "images/category_14.png" },
  { name: "Phiếu Quà", image: "images/category_15.png" },
  { name: "Nhãn Dán", image: "images/category_16.png" },
  { name: "Mác Sản", image: "images/category_17.png" },
  { name: "Giấy Ghi Chú", image: "images/category_18.png" },
];
</script>

<style scoped>
/* Optional custom styles */
</style>
