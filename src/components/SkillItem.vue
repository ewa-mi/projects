<template>
  <div>
    <img class="skill-item" :src="`${skill.svg}`" :title="`${skill.name}`" />
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
  height: 55px;
  margin: 9px;
}
</style>
