<template>
  <div class="footerItemsArea">
    <div class="footer-item">
      <a :href="`${footer.url}`" target="_blank" class="fooName">
        <img :src="`${footer.svg}`" />
      </a>
    </div>
  </div>
</template>

<script lang="ts">
export default {
  name: "FooterItem",
  props: ["footer"],
};
</script>

<style scoped>
.footer-item {
  width: 80px;
  height: 80px;
  margin-bottom: 10px;
  padding-top: 12px;
}

.footerItemsArea {
  display: flex;
  justify-content: center;
}
</style>
