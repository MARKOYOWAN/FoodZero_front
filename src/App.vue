<template>
  <HeaderPage />
  <FooterPage />
</template>

<script>
import HeaderPage from "./components/HeaderPage.vue";
import FooterPage from "./components/FooterPage.vue";

export default {
  name: "App",
  components: {
    HeaderPage,
    FooterPage,
  },
};
</script>

<style></style>
