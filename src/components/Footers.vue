<template>
  <div>
    <div v-bind:key="footer.id" v-for="footer in footers">
      <FooterItem v-bind:footer="footer" />
    </div>
  </div>
</template>

<script>
import FooterItem from "./FooterItem.vue";

export default {
  name: "Footer",
  components: {
    FooterItem,
  },
  props: ["footers"],
};
</script>

<style scoped></style>
