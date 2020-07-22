<template>
  <div>
    <div
      v-bind:key="project.id"
      v-for="project in projects"
      class="card-area-wrapper"
    >
      <ProjectItem v-bind:project="project" />
    </div>
  </div>
</template>

<script>
import ProjectItem from "./ProjectItem.vue";

export default {
  name: "Project",
  components: {
    ProjectItem,
  },
  props: ["projects"],
};
</script>

<style scoped>
.card-area-wrapper {
  margin-bottom: 23px;
}
</style>
