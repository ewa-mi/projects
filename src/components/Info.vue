<template>
  <div>
    <div class="card">
      <span class="card__infoicon">
        <h4 class="fa-info">ABOUT</h4>
      </span>
      <h1 class="card__title">About me</h1>
      <p class="card__description">
        Hi! My name is Ewa.
        <br />
        I’m a junior full-stack developer with a background in media
        communication and a few years of experience in graphic design. Highly
        driven and passionate about modern JavaScript and CSS tooling.
        <br />
        <br />
        I created this simple Vue app to show you my recent apps - MVPs. If you
        want to see more of my works, visit
        <a
          class="card__reference"
          href="https://github.com/ewa-mi"
          target="_blank"
          >my Github</a
        >
        !
      </p>
    </div>
  </div>
</template>

<script></script>

<style scoped>
.card {
  position: relative;
  padding: 32px 32px;
  clip-path: circle(50px at calc(100% - 51px) 50px);
  transition: all ease-in-out 0.4s;
  background-color: white;
  cursor: pointer;
}
.card__infoicon {
  position: absolute;
  top: 0;
  right: 0;
  padding: 40px 15px;
  background: white;
  font-size: 20px;
  color: #242a2e;
  transition: ease-out 0.2s;
  font-style: normal;
}
.card__title {
  margin: 0;
  font-size: 30px;
  line-height: 1.8;
  color: #242a2e;
}
.card__description {
  padding-top: 10px;
  margin: 0;
  font-size: 1em;
  line-height: 1.6;
  color: #242a2e;
}

.card__reference {
  display: inline-block;
  border-bottom: 1px solid transparent;
  color: #09f;
  text-decoration: none;
  transition: ease-in 0.4s;
}
.card__reference:hover {
  border-bottom-color: #09f;
}
.card:hover,
.card:focus {
  clip-path: circle(85%);
  border-radius: 12px;
  box-shadow: 0px 3px 9px rgba(0, 0, 0, 0.12), 0px 3px 18px rgba(0, 0, 0, 0.08);
  background: #fff;
  outline: none;
}
.card:hover .card__infoicon,
.card:focus .card__infoicon {
  opacity: 0;
}

@media (max-width: 768px) {
  .card {
    clip-path: none;
    transition: none;
    border-radius: 12px;
    background: none;
    padding-top: 0px;
  }
  .card__description,
  .card__title {
    color: white;
    text-align: center;
    max-width: 350px;
    margin: 0 auto;
  }
  .card__infoicon {
    display: none;
  }
  .card:hover,
  .card:focus {
    clip-path: none;
    border-radius: none;
    box-shadow: none;
    background: none;
    cursor: auto;
  }
}
@media (max-width: 375px) {
  .card__description,
  .card__title {
    max-width: 280px;
  }
}
</style>
