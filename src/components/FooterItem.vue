<template>
  <a :href="`${footer.url}`" target="_blank">
    <img class="footer-item" :src="`${footer.svg}`" />
  </a>
</template>

<script lang="ts">
export default {
  name: "FooterItem",
  props: ["footer"],
};
</script>

<style scoped>
.footer-item {
  width: 60px;
  height: 60px;
  margin: 5px;
  margin-bottom: 25px;
  padding-top: 12px;
}

.footer-item:hover {
  transition: ease-out 0.3s;
  filter: grayscale(100%) brightness(100%);
}
</style>
