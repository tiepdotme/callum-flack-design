<template>
  <div class="AboutServices frame frame--columns text-gray-dark">
    <div class="grid-area-a">
      <h2>{{ design.title }}</h2>
      <p>{{ design.lede }}</p>
      <ul>
        <li v-for="(item, index) in design.items" :key="index">{{ item }}</li>
      </ul>
    </div>
    <div class="grid-area-b">
      <h2>{{ dev.title }}</h2>
      <p>{{ dev.lede }}</p>
      <ul>
        <li v-for="(item, index) in dev.items" :key="index">{{ item }}</li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  data: () => ({
    design: {
      title: "Thanh toán chuyển khoản",
      lede:
        "mình chỉ sử dụng duy nhất tài khoản ngân hàng mở tại Vietcombank thông tin thanh toán chi tiết bên dưới.",
      /* Designed to work, without losing the sense of ease that good craft delivers. */
      items: [
        "Phạm Xuân Tiếp",
        "0281000538644",
        "Ngân hàng Vietcombank",
      ],
    },
    dev: {
      title: "Development",
      lede:
        "Our focus is the web. We use modern tools to build performant, secure sites that are easy to iterate. We design in code to prototype how products feel.",
      items: [
        "Frontend web development",
        "API creation and integration",
        "Serverless functions",
        "Backend managment",
      ],
    },
  }),
};
</script>

<style lang="postcss">
.AboutServices h2 {
  @apply mt-0 !important;
}
</style>
