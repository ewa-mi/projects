<template>
  <div>
    <img class="skill-item" :src="`${skill.svg}`" />
  </div>
</template>

<script>
export default {
  name: "SkillItem",
  props: ["skill"],
};
</script>

<style scoped>
.skill-item {
  width: 60px;
  height: 60px;
  margin: 10px;
  padding-top: 10px;
}
</style>
