<template>
  <div class="cards-area">
    <div class="project-item">
      <h1>{{ project.title }}</h1>
      <p>{{ project.tech }}</p>
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
  border: 5px coral solid;
  border-radius: 12px;
  width: 250px;
  margin-bottom: 20px;
}

.del {
  background: peru;
  color: whitesmoke;
  border: none;
  padding: 5px 9px;
  border-radius: 50%;
  cursor: pointer;
  float: right;
}
</style>
