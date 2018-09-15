<template>
  <section class="container">
    <div class="mission">
      <div class="mission-statement title">
        aksdfjdsljf
      </div>
      <div class="mission-description subtitle">
        kjadsfkljs
      </div>
    </div>
  </section>
</template>

<style lang="css" scoped>
.mission {
  min-height: 100vh;
  min-width: 100vw;
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  grid-template-rows: repeat(2, 1fr);
  grid-template-areas: "statement img" "description img";
  justify-content: center;
  align-items: center;
  background-color: #d8ab4c;
}

.mission-statement {
  grid-area: statement;
}

.mission-description {
  grid-area: description;
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
</style>
