<template>
  <div id="app">
    <Header />
    <div class="grid">
      <Info />
      <Projects v-bind:projects="projects" />
    </div>
    <Footers v-bind:footers="footers" />
  </div>
</template>

<script>
import Header from "./components/layout/Header";
import Info from "./components/Info";
import Projects from "./components/Projects";
import Footers from "./components/Footers";
import bookapp from "./components/images/bookapp.png";
import click from "./components/images/click.png";
import cosmos from "./components/images/cosmos.png";

export default {
  name: "app",
  components: {
    Header,
    Info,
    Projects,
    Footers,
  },
  data() {
    return {
      projects: [
        {
          id: 1,
          title: "Book App",
          tech: "React-Redux, Node",
          linkGithub: "https://github.com/ewa-mi/book-app-client",
          linkWebsite: "https://book-app-portfolio.netlify.app/",
          img: bookapp,
        },
        {
          id: 2,
          title: "Click the Pic",
          tech: "React-Redux, Node",
          linkGithub: "https://github.com/ewa-mi/clicthepic_FE",
          linkWebsite: "https://clickthepic.netlify.app",
          img: click,
        },
        {
          id: 3,
          title: "Out of This World",
          tech: "React, Bootstrap",
          linkGithub: "https://github.com/ewa-mi/feed_in_react",
          linkWebsite: "https://out-of-this-world-react-app.netlify.app",
          img: cosmos,
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
  font-family: "Lucida Sans", "Lucida Sans Regular", "Lucida Grande",
    "Lucida Sans Unicode", Geneva, Verdana, sans-serif;
  line-height: 1;

  background-color: rgb(24, 24, 24);
}

.grid {
  display: grid;
  grid-template-columns: 1fr 2fr 1fr;
  grid-gap: 20px;
  padding: 18px;
}
</style>
