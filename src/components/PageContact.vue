<template>
  <div>
    <h2 class="Heading Heading-4xl font-medium">Tiếp adsense</h2>
    <p class="Space-t mb-2px">{{ about }}</p>
    <p class="Text Link mb-2px">
      <a :href="`mailto:${contact.email}`">
        <span class="Text-contact-type">E: </span>
        <span>{{ contact.email }}</span>
      </a>
    </p>
    <p class="Text Link">
      <a :href="`tel:0${contact.phone.replace(/ /g, '-')}`">
        <span class="Text-contact-type">T: </span>
        <span>+61(0) {{ contact.phone }}</span>
      </a>
    </p>
    <div class="Space-y">
      <p class="Text mb-2px">{{ signup }}</p>
      <FormNewsletter></FormNewsletter>
    </div>
    <p class="Text-xs text-gray-dark">
      © Tiếp adsense 2015–{{ new Date().getFullYear() }}
    </p>
  </div>
</template>

<script>
import FormNewsletter from "../components/FormNewsletter";

export default {
  components: {
    FormNewsletter,
  },
  props: {},
  data: () => ({
    about: "Để liên lạc với Tiếp:",
    signup: "Để làm việc lâu dài và nhận giá ưu đãi:",
    contact: {
      email: "tiep@kadao.me",
      phone: "0702227255",
    },
  }),
};
</script>

<style lang="postcss" scoped>
.Text-contact-type {
  @apply inline-block;
  font-size: 85%;
  width: 1.2em;
}
</style>
