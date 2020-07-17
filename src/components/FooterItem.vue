<template>
  <div>
    <div class="footer-item">
      <a :href="`${footer.url}`" target="_blank" class="fooName">{{
        footer.name
      }}</a>
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
  background: rgb(245, 245, 244);
  border: 2px white solid;
  border-radius: 5px;
  width: 130px;
  height: 70px;
  margin-bottom: 6px;
  padding-top: 12px;
  text-align: center;
}

.fooName {
  font-size: 30px;
  color: rgb(21, 21, 21);
  text-decoration: none;
}
</style>
