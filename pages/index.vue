<template>
  <section class="container">
    <div class="home">
      <img src="../static/vt-logo.svg" class="logo">
      <p class="title">
        We empower communicators.
      </p>
    </div>
    <Mission></Mission>
  </section>
</template>

<script>
import AppLogo from "~/components/AppLogo.vue";
import Mission from "~/components/Mission.vue";

export default {
  components: {
    AppLogo,
    Mission
  }
};
</script>

<style>
body {
  max-width: 100vw;
  overflow-x: hidden;
}

.container {
  min-height: 100vh;
  display: flex;
  flex-flow: column nowrap;
  justify-content: center;
  align-items: center;
  text-align: center;
  background-color: white;
}

.home {
  min-height: 100vh;
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  justify-content: center;
  align-items: center;
}

.title {
  font-family: Roboto, "Quicksand", "Source Sans Pro", -apple-system,
    BlinkMacSystemFont, "Segoe UI", "Helvetica Neue", Arial, sans-serif;
  /* 1 */
  font-weight: 330;
  font-size: 3em;
  color: black;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 330;
  font-size: 2em;
  color: black;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}

.logo {
  width: 40vh;
  height: 40vh;
  align-self: center;
  animation: turn 2s linear forwards 1s;
  grid-column: 2 / 3;
}

@keyframes turn {
  100% {
    transform: rotateY(360deg);
  }
}

@keyframes godown {
  100% {
    top: 180px;
  }
}

@keyframes goright {
  100% {
    left: 70px;
  }
}
</style>
