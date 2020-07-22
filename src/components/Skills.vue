<template>
  <div>
    <div v-bind:key="skill.id" v-for="skill in skills">
      <SkillItem v-bind:skill="skill" />
    </div>
  </div>
</template>

<script>
import SkillItem from "./SkillItem.vue";

export default {
  name: "Skill",
  components: {
    SkillItem,
  },
  props: ["skills"],
};
</script>

<style scoped></style>
