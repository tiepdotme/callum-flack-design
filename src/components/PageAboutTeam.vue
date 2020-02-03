<template>
  <div class="AboutTeam frame frame--columns Block-sm-t">
    <div class="grid-area-a">
      <div class="md:w-1/2 lg:w-6/12 Space">
        <ImageDynamic ratio="12/10" :src="callum.portrait" />
      </div>
      <div class="text-gray-dark">
        <h2>{{ callum.name }}</h2>
        <h3>{{ callum.title }}</h3>
        <p v-html="callum.lede"></p>
        <ul class="Text-sm">
          <li class="mb-0">
            <a :href="`mailto:${callum.contacts.email}`">
              Email: {{ callum.contacts.email }}
            </a>
          </li>
          <li>
            <a :href="`tel:0${callum.contacts.phone.replace(/ /g, '-')}`">
              Call: +84(0) {{ callum.contacts.phone }}
            </a>
          </li>
          <li>
            <a
              :href="`www.linkedin.com/in/${callum.contacts.linkedin}`"
              target="_blank"
              rel="noopener noreferrer"
            >
              Callum on Linkedin
            </a>
          </li>
          <li>
            <a
              :href="`https://github.com/${callum.contacts.github}`"
              target="_blank"
              rel="noopener noreferrer"
            >
              Callum on Github
            </a>
          </li>
        </ul>
      </div>
    </div>
    <div class="grid-area-b">
      <div class="md:w-1/2 lg:w-6/12 Space">
        <ImageDynamic ratio="12/10" :src="barry.portrait" />
      </div>
      <div class="text-gray-dark">
        <h2>{{ barry.name }}</h2>
        <h3>{{ barry.title }}</h3>
        <p v-html="barry.lede"></p>
        <ul class="Text-sm">
          <li class="mb-0">
            <a :href="`mailto:${barry.contacts.email}`">
              Email: {{ barry.contacts.email }}
            </a>
          </li>
          <li>
            <a
              :href="`https://github.com/${barry.contacts.github}`"
              target="_blank"
              rel="noopener noreferrer"
            >
              Barry on Github
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
    callum: {
      name: "Phạm Tiếp",
      title: "Bán hàng, tạo tài khoản, bảo hành",
      portrait: "/images/tiep.jpg",
      lede:
        "Tiếp đã dành trọn cuộc sống của mình để tìm kiếm cái đẹp và tạo ra sản phẩm có giá trị, kể từ năm 2006 đã có duyên gắn bó với nghề và đi lên bằng bán tài khoản download, sau này khi PTU đi xuống, mình chuyển hướng sang adsense và đạt được một số thành công nhất định, mình hy vọng mình có thể tạo ra nhiều sản phẩm hơn để phục vụ mọi người chu đáo cho công việc quảng cáo online trực tuyến thông qua web và ứng dụng.",
      contacts: {
        email: "tiep@kadao.me",
        phone: "408 767 540",
        linkedin: "dekadao",
        github: "dekadao",
      },
    },
    barry: {
      name: "Linh",
      title: "Backend",
      portrait: "/images/linh.jpg",
      lede:
        "Là một người bạn đồng hành đáng tin cậy, và xứng đáng để kết bạn.",
      contacts: {
        email: "linh@kadao.me",
        github: "linhkadao",
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
