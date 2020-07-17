<template>
  <div id="app">
    <Header />
    <Projects v-bind:projects="projects" />
    <Footers v-bind:footers="footers" />
  </div>
</template>

<script>
import Header from "./components/layout/Header";
import Projects from "./components/Projects";
import Footers from "./components/Footers";

export default {
  name: "app",
  components: {
    Header,
    Projects,
    Footers,
  },
  data() {
    return {
      projects: [
        {
          id: 1,
          title: "Out of This World",
          tech: "React",
          linkGithub: "https://github.com/ewa-mi/feed_in_react",
          linkWeb: "https://out-of-this-world-react-app.netlify.app",
        },
        {
          id: 2,
          title: "Book App",
          tech: "React-Redux, Node",
          linkGithub: "https://github.com/ewa-mi/book-app-client",
          linkWeb: "https://book-app-portfolio.netlify.app/",
        },
        {
          id: 3,
          title: "Click the Pic",
          tech: "React-Redux, Node",
          linkGithub: "https://github.com/ewa-mi/clicthepic_FE",
          linkWeb: "https://clickthepic.netlify.app",
        },
      ],
      footers: [
        {
          id: 1,
          name: "Github",
          url: "https://www.github.com/ewa-mi",
        },
        {
          id: 2,
          name: "LinkedIn",
          url: "https://www.linkedin.com/in/ewa-michalowska-b8429b78/",
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

  background-color: rgb(24, 24, 24);
}
</style>
