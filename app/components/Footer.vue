<template>
  <footer class="bg-gray-900 text-white py-10 px-4">
    <div class="max-w-screen-xl mx-auto grid grid-cols-1 md:grid-cols-3 gap-8">
      <!-- About -->
      <div>
        <h3 class="text-xl font-semibold mb-4">Về Chúng Tôi</h3>
        <p class="text-gray-300 text-sm leading-relaxed">
          Chuyên cung cấp ấn phẩm quảng cáo, in băng rôn, tờ rơi, standee,
          backdrop và các dịch vụ in ấn chuyên nghiệp tại Xã Phước Hòa, Huyện
          Phú Giáo, Bình Dương.
        </p>
      </div>

      <!-- Services -->
      <div>
        <h3 class="text-xl font-semibold mb-4">Dịch Vụ</h3>
        <ul class="text-gray-300 text-sm space-y-2">
          <li>📌 Thiết kế & In ấn băng rôn</li>
          <li>📌 In tờ rơi - leaflet</li>
          <li>📌 Standee - Backdrop sự kiện</li>
          <li>📌 Nhận in số lượng ít & gấp</li>
        </ul>
      </div>

      <!-- Contact -->
      <div>
        <h3 class="text-xl font-semibold mb-4">Liên Hệ</h3>
        <ul class="text-gray-300 text-sm space-y-2">
          <li>📍 Địa chỉ: Xã Phước Hòa, Phú Giáo, Bình Dương</li>
          <li>
            📞 Điện thoại:
            <a href="tel:0937704598" class="text-blue-400 hover:underline"
              >0937 704 598</a
            >
          </li>
          <li>
            📧 Email:
            <a
              href="mailto:tanthanh1998.phuochoa@gmail.com"
              class="text-blue-400 hover:underline"
              >tanthanh1998.phuochoa@gmail.com</a
            >
          </li>
          <li>🕒 Giờ làm việc: 8:00 – 18:00 (T2–T7)</li>
        </ul>
      </div>
    </div>

    <!-- Bottom -->
    <div
      class="mt-10 text-center text-gray-500 text-sm border-t border-gray-700 pt-6"
    >
      © {{ new Date().getFullYear() }} Phước Hòa Print. All rights reserved.
    </div>
  </footer>
</template>

<script setup>
// No script needed for now
</script>

<style scoped>
/* Optional: add hover underline for all links inside footer */
a:hover {
  text-decoration: underline;
}
</style>
