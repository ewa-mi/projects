<template>
  <div class="cards-area">
    <div class="project-item">
      <h1 class="projectText">{{ project.title }}</h1>
      <p class="techText">{{ project.tech }}</p>
      <div class="proLinksArea">
        <a class="proLink" :href="`${project.linkGithub}`" target="_blank"
          >CODE</a
        >
        <a class="proLink" :href="`${project.linkWebsite}`" target="_blank"
          >WEBSITE</a
        >
      </div>
    </div>
    <div>
      <img class="demoImg" :src="`${project.img}`" />
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
  border-top-left-radius: 12px;
  border-bottom-left-radius: 12px;
  border-right: none;

  width: 320px;
  height: 320px;
  margin-bottom: 20px;
}

.projectText {
  text-align: center;
  margin-bottom: 15px;
  margin-top: 40px;
}
.techText {
  text-align: center;
  margin-bottom: 55px;
}

.proLinksArea {
  margin-top: 65px;
  text-align: center;
}
.proLink {
  padding: 10px;
  text-decoration: none;
  color: rgb(23, 23, 23);
  background: white;
  border: 2px white solid;
  border-radius: 5px;
  margin-left: 7px;
}

.demoImg {
  height: 320px;
  border: 5px white solid;
  border-top-right-radius: 12px;
  border-bottom-right-radius: 12px;
  border-left: none;
}
</style>
