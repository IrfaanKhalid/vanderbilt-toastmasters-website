<template>
  <section class="container">
    <div>
      <img src = "../static/logo-orig.jpg" class="logo">
      <h1 class="title">
        Welcome to Vanderbilt Toastmasters!
      </h1>
      <h2 class="subtitle">
        We meet at 6pm on the 2nd and 4th Wednesday of every month in Buttrick Hall 301.
      </h2>
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
  justify-content: center;
  align-items: center;
  text-align: center;
  background-color: #866d4b;
}

.title {
  font-family: Roboto, "Quicksand", "Source Sans Pro", -apple-system,
    BlinkMacSystemFont, "Segoe UI", "Helvetica Neue", Arial, sans-serif; /* 1 */
  display: block;
  font-weight: 330;
  font-size: 5em;
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
  border-radius : 50%;
  width: 40vh;
  height: 40vh;
}
</style>
