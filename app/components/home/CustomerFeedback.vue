<template>
  <section class="py-20 bg-white">
    <div class="max-w-7xl mx-auto px-4">
      <!-- Tiêu đề -->
      <div class="text-center mb-12">
        <h2 class="text-3xl md:text-4xl font-bold text-red-500">
          Cảm Nhận Khách Hàng Khi Dùng Dịch Vụ In Ấn
        </h2>
        <div class="mt-2 w-20 h-1 bg-red-500 mx-auto"></div>
      </div>

      <!-- Danh sách đánh giá -->
      <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
        <div
          v-for="(feedback, index) in feedbacks"
          :key="index"
          class="bg-white p-6 rounded-2xl shadow-sm border text-gray-700 space-y-4 hover:shadow-lg transition"
        >
          <!-- Nội dung -->
          <p class="italic">"{{ feedback.text }}"</p>

          <!-- Rating -->
          <div class="text-red-500 text-sm">
            <span v-for="i in 5" :key="i">
              <i class="fas fa-star"></i>
            </span>
          </div>

          <!-- Người dùng -->
          <div class="flex items-center gap-3 pt-2">
            <img
              :src="feedback.avatar"
              alt="avatar"
              class="w-10 h-10 rounded-full object-cover"
            />
            <div class="text-sm font-bold text-red-500 flex items-center gap-1">
              {{ feedback.name }}
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
const feedbacks = [
  {
    text: "Băng rôn được in sắc nét, đúng màu, giao đúng hẹn cho sự kiện khai trương. Sẽ tiếp tục ủng hộ!",
    name: "Chị Lan (Xã Phước Hòa)",
    avatar: "images/avt_1.png",
  },
  {
    text: "Dịch vụ in name card cực kỳ nhanh và chuyên nghiệp. Mẫu thiết kế đẹp, giấy in chất lượng cao.",
    name: "Anh Hoàng (Phú Giáo)",
    avatar: "images/avt_2.png",
  },
  {
    text: "Tôi đặt in áo thun đồng phục, chất vải tốt, in logo rõ nét. Giá cả hợp lý, phục vụ tận tâm.",
    name: "Chị Mai (Bình Dương)",
    avatar: "images/avt_3.png",
  },
];
</script>

<style scoped>
@import url("https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css");
</style>
