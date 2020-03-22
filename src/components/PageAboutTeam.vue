<template>
  <div class="AboutTeam frame frame--columns Block-sm-t">
    <div class="grid-area-a">
      <div class="md:w-1/2 lg:w-6/12 Space">
        <ImageDynamic ratio="12/10" :src="tiep.portrait" />
      </div>
      <div class="text-gray-dark">
        <h2>{{ tiep.name }}</h2>
        <h3>{{ tiep.title }}</h3>
        <p v-html="tiep.lede"></p>
        <ul class="Text-sm">
          <li class="mb-0">
            <a :href="`mailto:${tiep.contacts.email}`">
              Email: {{ tiep.contacts.email }}
            </a>
          </li>
          <li>
            <a :href="`tel:${tiep.contacts.phone.replace(/ /g, '-')}`">
              Call: +84 {{ tiep.contacts.phone }}
            </a>
          </li>
          <li>
            <a
              :href="`www.linkedin.com/in/${tiep.contacts.linkedin}`"
              target="_blank"
              rel="noopener noreferrer"
            >
              Tiếp trên Linkedin
            </a>
          </li>
          <li>
            <a
              :href="`https://facebook.com/${tiep.contacts.facebook}`"
              target="_blank"
              rel="noopener noreferrer"
            >
              Tiếp trên Facebook
            </a>
          </li>
        </ul>
      </div>
    </div>
    <div class="grid-area-b">
      <div class="md:w-1/2 lg:w-6/12 Space">
        <ImageDynamic ratio="12/10" :src="hong.portrait" />
      </div>
      <div class="text-gray-dark">
        <h2>{{ hong.name }}</h2>
        <h3>{{ hong.title }}</h3>
        <p v-html="hong.lede"></p>
        <ul class="Text-sm">
          <li class="mb-0">
            <a :href="`mailto:${hong.contacts.email}`">
              Email: {{ hong.contacts.email }}
            </a>
          </li>
          <li>
            <a
              :href="`https://facebook.com/${hong.contacts.facebook}`"
              target="_blank"
              rel="noopener noreferrer"
            >
              Tôi trên Facebook
            </a>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
import ImageDynamic from "../components/ImageDynamic";

export default {
  components: {
    ImageDynamic,
  },
  data: () => ({
    tiep: {
      name: "Phạm Tiếp",
      title: "Bán hàng, tạo tài khoản, bảo hành",
      portrait: "/images/tiep.jpg",
      lede:
        "Tiếp đã dành trọn cuộc sống của mình để tìm kiếm cái đẹp và tạo ra sản phẩm có giá trị, kể từ năm 2006 đã có duyên gắn bó với nghề và đi lên bằng bán tài khoản download, sau này khi PTU đi xuống, mình chuyển hướng sang adsense và đạt được một số thành công nhất định, mình hy vọng mình có thể tạo ra nhiều sản phẩm hơn để phục vụ mọi người chu đáo cho công việc quảng cáo online trực tuyến thông qua web và ứng dụng.",
      contacts: {
        email: "tiep@kadao.me",
        phone: "0702227255",
        linkedin: "dekadao",
        facebook: "tiepmatkieng",
      },
    },
    hong: {
      name: "Tôi tuổi 24",
      title: "Backend",
      portrait: "/images/tiep2.jpg",
      lede:
        "Tôi thường chụp hình khi buồn một mình và để khuôn mặt cười tươi.",
      contacts: {
        email: "tiep@kadao.me",
        facebook: "tiepmatkieng",
      },
    },
  }),
};
</script>

<style lang="postcss">
.AboutTeam {
  /* margin-bottom: calc(theme(spacing.2) * var(--space-ratio)) !important; */
  grid-row-gap: var(--spacing5);
}
.AboutTeam h2 {
  @apply mt-0 mb-2px !important;
  /* margin-bottom: calc(theme(spacing.2) * var(--space-ratio)) !important; */
}
.AboutTeam h3 {
  @apply mt-0 !important;
  font-size: calc(theme(fontSize.sm) * var(--text-ratio));
}
/* .AboutTeam li:before {
  --markdown-text-indent: 0;
  content: initial;
} */
</style>
