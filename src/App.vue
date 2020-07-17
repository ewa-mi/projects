<template>
  <div id="app">
    <Projects v-bind:projects="projects" />
  </div>
</template>

<script>
import Projects from "./components/Projects";

export default {
  name: "app",
  components: {
    Projects,
  },
  data() {
    return {
      projects: [
        {
          id: 1,
          title: "Universe",
          tech: "React",
        },
        {
          id: 2,
          title: "Book App",
          tech: "React-Redux, Node",
        },
        {
          id: 3,
          title: "Click the Pic",
          tech: "React-Redux, Node",
        },
      ],
    };
  },
};
</script>

<style>
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

body {
  font-family: Arial, Helvetica, sans-serif;
  line-height: 1.5;
}
</style>
