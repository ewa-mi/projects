<template>
  <div class="cards-area">
    <div class="project-item">
      <h1 class="projectText">{{ project.title }}</h1>
      <p class="techText">{{ project.tech }}</p>
    </div>
  </div>
</template>

<script lang="ts">
export default {
  name: "ProjectItem",
  props: ["project"],
};
</script>

<style scoped>
.cards-area {
  display: flex;
  justify-content: center;
  margin-top: 50px;
}

.project-item {
  background: greenyellow;
  padding: 20px;
  border: 5px white solid;
  border-radius: 12px;
  width: 250px;
  height: 250px;
  margin-bottom: 20px;
}

.projectText,
.techText {
  text-align: center;
}
</style>
