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
              :href="`https://www.linkedin.com/in/${tiep.contacts.linkedin}`"
              target="_blank"
              rel="noopener noreferrer"
            >
              Psm trên Linkedin
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
        <ImageDynamic ratio="12/10" :src="psm.portrait" />
      </div>
      <div class="text-gray-dark">
        <h2>{{ psm.name }}</h2>
        <h3>{{ psm.title }}</h3>
        <p v-html="psm.lede"></p>
        <ul class="Text-sm">
          <li class="mb-0">
            <a :href="`mailto:${psm.contacts.email}`">
              Email: {{ psm.contacts.email }}
            </a>
          </li>
          <li>
            <a
              :href="`https://facebook.com/${psm.contacts.facebook}`"
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
      name: "Psm Tiếp",
      title: "Sáng lập,  Bán hàng, tạo tài khoản, bảo hành",
      portrait: "/images/tiep_2020.png",
      lede:
        "Tiếp (Psm) chuyên tạo tài khoản kể từ năm 2006 đã có duyên gắn bó với nghề và đi lên bằng bán tài khoản download, sau này khi PTU đã không còn ở đỉnh điểm của chú ý, mình rẽ hướng sang AdSense, muốn tạo ra các tài khoản giúp các bạn có thêm phương án làm việc tại nhà đảm bảo nguồn thu cho gia đình riêng.",
      contacts: {
        email: "Psm@phusa.me",
        phone: "(033) 703-6819",
        linkedin: "phusame",
        facebook: "100050845217346",
      },
    },
    psm: {
      name: "Psm Children",
      title: "Backend, Kế thừa, Frontend, Developer",
      portrait: "/images/tiep2.jpg",
      lede:
        "Kế thừa và phát triển Psm trở nên lớn mạnh và đa dạng hơn tương tự như một Agency đích thực.",
      contacts: {
        email: "tiep@phusa.me",
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
