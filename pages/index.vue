<template>
  <section class="container">
    <div class="home">
      <img src="../static/vt-logo.svg" class="logo">
      <p class="title">
        Where leaders are made.
      </p>
    </div>
  </section>
</template>

<script>
import AppLogo from "~/components/AppLogo.vue";

export default {
  components: {
    AppLogo
  }
};
</script>

<style>
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

.page {
  min-height: 100vh;
  display: grid;
  flex-flow: column nowrap;
  justify-content: center;
  align-content: center;
}

.title {
  font-family: Roboto, "Quicksand", "Source Sans Pro", -apple-system,
    BlinkMacSystemFont, "Segoe UI", "Helvetica Neue", Arial, sans-serif;
  /* 1 */
  display: block;
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
  grid-column: 3 / 4;
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
