<template>
  <div>
    <div class="footer-item">
      <h1 class="fooName">{{ footer.name }}</h1>
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
  width: 150px;
  height: 80px;
  margin-bottom: 6px;
  padding-top: 15px;
}

.fooName {
  text-align: center;
}
</style>
