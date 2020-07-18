<template>
  <div class="card" tabindex="0">
    <span class="card__infoicon">
      <h4 class="fa fa-info">ABOUT</h4>
    </span>
    <h1 class="card__title">About me</h1>
    <p class="card__description">
      Hi! My name is Ewa.
      <br />
      I’m a junior full-stack developer with a background in media communication
      and a few years of experience in graphic design. Highly driven and
      passionate about modern JavaScript and CSS.
      <br />
      <br />
      I created this Vue app to show you my recent projects. If you want to see
      more of my works, visit
      <a
        class="card__reference"
        href="https://github.com/ewa-mi"
        target="_blank"
        >my Github</a
      >
      !
    </p>
  </div>
</template>

<script></script>

<style scoped>
.card {
  position: relative;
  height: 500px;
  padding: 32px 32px;
  margin-top: 49px;
  clip-path: circle(11% at 84% 10%);
  transition: all ease-in-out 0.4s;
  background-color: white;
  cursor: pointer;
}
.card__infoicon {
  position: absolute;
  top: 40px;
  right: 22px;
  font-size: 20px;
  color: #242a2e;
  transition: ease-out 0.4s;
  font-style: normal;
}
.card__title {
  margin: 0;
  font-size: 40px;
  line-height: 1.8;
  color: #242a2e;
}
.card__description {
  margin: 0;
  font-size: 1.1em;
  line-height: 1.6;
  color: #242a2e;
}

.card__reference {
  display: inline-block;
  border-bottom: 1px solid transparent;
  color: #09f;
  text-decoration: none;
  transition: ease-in 0.3s;
}
.card__reference:hover {
  border-bottom-color: #09f;
}
.card:hover,
.card:focus {
  clip-path: circle(85%);
  border-radius: 20px;
  box-shadow: 0px 3px 9px rgba(0, 0, 0, 0.12), 0px 3px 18px rgba(0, 0, 0, 0.08);
  background: #fff;
  outline: none;
}
.card:hover .card__infoicon,
.card:focus .card__infoicon {
  opacity: 0;
}
.card:focus {
  box-shadow: 0px 3px 9px rgba(0, 0, 0, 0.12), 0px 3px 18px rgba(0, 0, 0, 0.08),
    0px 0px 0px 4px rgba(0, 0, 0, 0.2);
}
</style>
