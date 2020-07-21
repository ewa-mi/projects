<template>
  <div id="app">
    <Header />
    <div class="grid">
      <Info />
      <Projects v-bind:projects="projects" class="projects" />
      <div class="rightSidebarWrapper">
        <div class="rightSidebar">
          <h1 class="tech">TECH</h1>
          <Skills v-bind:skills="skills" class="skills" />
        </div>
      </div>
    </div>
    <Footers v-bind:footers="footers" class="footers" />
  </div>
</template>

<script>
import Header from "./components/layout/Header";
import Info from "./components/Info";
import Projects from "./components/Projects";
import Skills from "./components/Skills";
import Footers from "./components/Footers";
//assets:
import bookapp from "./components/images/bookapp.png";
import click from "./components/images/click.png";
import cosmos from "./components/images/cosmos.png";
import github from "./components/layout/github.svg";
import linkedin from "./components/layout/linkedin.svg";
import docker from "./components/tech-icons/docker.svg";
import bootstrap from "./components/tech-icons/bootstrap.svg";
import css from "./components/tech-icons/css.svg";
import git from "./components/tech-icons/git.svg";

export default {
  name: "app",
  components: {
    Header,
    Info,
    Projects,
    Skills,
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
          svg: github,
          url: "https://www.github.com/ewa-mi",
        },
        {
          id: 2,
          svg: linkedin,
          url: "https://www.linkedin.com/in/ewa-michalowska-b8429b78/",
        },
      ],
      skills: [
        {
          id: 1,
          svg: docker,
        },
        {
          id: 2,
          svg: bootstrap,
        },
        {
          id: 3,
          svg: css,
        },
        {
          id: 4,
          svg: git,
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
  margin-top: 50px;
}

.footers {
  display: flex;
  justify-content: center;
}

.rightSidebar {
  display: flex;
  flex-direction: column;
  background-color: white;
  border-radius: 12px;
  align-items: center;
  padding: 20px 0;
}

.tech {
  font-size: 21px;
  line-height: 1.8;
  color: #242a2e;
  text-align: center;
  padding-bottom: 10px;
}
</style>
