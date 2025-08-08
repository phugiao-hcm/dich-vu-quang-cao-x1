<template>
  <section class="py-8 px-4">
    <div class="max-w-screen-xl mx-auto">
      <!-- Header -->
      <div>
        <h2 class="text-4xl font-bold text-black mb-3">SẢN PHẨM NỔI BẬT</h2>
        <p class="text-gray-500 text-lg max-w-2xl">
          Các sản phẩm in ấn chất lượng cao, sắc nét và chuyên nghiệp – từ băng
          rôn quảng cáo, danh thiếp đến brochure, poster – giúp doanh nghiệp bạn
          nổi bật và gây ấn tượng mạnh với khách hàng.
        </p>
      </div>

      <!-- Category Tabs -->
      <div class="flex flex-wrap gap-2 my-6">
        <button
          v-for="(tab, index) in tabs"
          :key="index"
          :class="[
            'px-4 py-2 rounded font-medium',
            activeTab === tab
              ? 'bg-red-600 text-white'
              : 'bg-gray-100 text-gray-700',
          ]"
          @click="activeTab = tab"
        >
          {{ tab }}
        </button>
      </div>

      <!-- Product Grid -->
      <!-- Product Grid -->
      <div
        class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 xl:grid-cols-4 gap-6"
      >
        <div
          v-for="(product, index) in filteredProducts"
          :key="index"
          class="rounded-lg overflow-hidden shadow-md hover:shadow-xl transition"
        >
          <img
            :src="product.image"
            :alt="product.title"
            class="w-full h-48 object-cover"
          />
          <div class="p-4">
            <h3 class="text-sm font-medium text-gray-800 mb-2 leading-snug">
              {{ product.title }}
            </h3>
            <p class="text-red-600 font-semibold text-lg">
              {{ product.price }} đ
            </p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import { ref, computed } from "vue";

// Danh mục sản phẩm in ấn (có "Tất cả")
const tabs = [
  "Tất cả",
  "Băng rôn quảng cáo",
  "Standee - Poster",
  "Brochure - Tờ rơi",
  "Name card - Danh thiếp",
  "In bao thư - tiêu đề",
  "Tem nhãn sản phẩm",
  "In trên áo - mũ",
  "Catalogue - Hồ sơ năng lực",
];

const activeTab = ref("Tất cả");

// Danh sách sản phẩm giả lập (thay bằng API nếu có)
const products = ref([
  {
    title: "Băng rôn khuyến mãi khai trương 1.5m x 5m",
    price: "180.000",
    image: "images/banner_1.png",
    category: "Băng rôn quảng cáo",
  },
  {
    title: "Băng rôn in PP không cán, kháng nước",
    price: "220.000",
    image: "images/banner_2.png",
    category: "Băng rôn quảng cáo",
  },
  {
    title: "Standee 0.8m x 1.8m khung cuốn nhôm",
    price: "250.000",
    image: "images/banner_3.png",
    category: "Băng rôn quảng cáo",
  },
  {
    title: "Poster A3 in màu giấy couche 200gsm",
    price: "120.000",
    image: "images/banner_4.png",
    category: "Standee - Poster",
  },
  {
    title: "Tờ rơi quảng cáo A5 in 2 mặt giấy couche",
    price: "95.000",
    image: "images/banner_5.png",
    category: "Brochure - Tờ rơi",
  },
  {
    title: "Name card ép kim sang trọng",
    price: "180.000",
    image: "images/banner_6.png",
    category: "Name card - Danh thiếp",
  },
  {
    title: "In tem nhãn sản phẩm decal nhựa",
    price: "150.000",
    image: "images/banner_7.png",
    category: "Tem nhãn sản phẩm",
  },
  {
    title: "Catalogue giới thiệu doanh nghiệp 16 trang",
    price: "680.000",
    image: "images/banner_8.png",
    category: "Băng rôn quảng cáo",
  },
  {
    title: "Catalogue giới thiệu doanh nghiệp 16 trang 11",
    price: "680.000",
    image: "images/banner_9.png",
    category: "Catalogue - Hồ sơ năng lực",
  },
  {
    title: "Catalogue giới thiệu doanh nghiệp 16 trang 22",
    price: "680.000",
    image: "images/banner_10.png",
    category: "Catalogue - Hồ sơ năng lực",
  },
]);

const filteredProducts = computed(() => {
  if (activeTab.value === "Tất cả") return products.value;
  return products.value.filter((p) => p.category === activeTab.value);
});
</script>
