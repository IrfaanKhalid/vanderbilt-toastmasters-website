<template>
  <section class="container">
    <div class="mission">
      <div class="mission-statement title">
        Mission statement
      </div>
      <div class="mission-description subtitle">
        Mission description
      </div>
      <img class="mission-img" src="../static/mission.png" />
    </div>
  </section>
</template>

<style lang="css" scoped>
.mission {
  min-height: 100vh;
  max-height: 100vh;
  min-width: 100vw;
  display: grid;
  justify-content: center;
  align-items: center;
  grid-template-columns: repeat(2, 1fr);
  grid-template-rows: repeat(2, 1fr);
  grid-template-areas: "statement img" "description img";
  background-color: #d8ab4c;
}

.mission-statement {
  grid-area: statement;
  justify-content: center;
  text-align: center;
  margin-left: 5vw;
  margin-right: 5vw;
  filter: drop-shadow(5px 5px 10px black);
}

.mission-description {
  grid-area: description;
  justify-content: center;
  text-align: center;
  margin-left: 5vw;
  margin-right: 5vw;
}

.mission-img {
  grid-area: img;
  image-rendering: crisp-edges;
}

.title {
  font-family: Roboto, "Quicksand", "Source Sans Pro", -apple-system,
    BlinkMacSystemFont, "Segoe UI", "Helvetica Neue", Arial, sans-serif;
  /* 1 */
  font-weight: 330;
  font-size: 3em;
  color: black;
  letter-spacing: 1px;
  font-style: italic;
}

.subtitle {
  font-weight: 330;
  font-size: 2em;
  color: black;
  word-spacing: 5px;
  padding-bottom: 15px;
}
</style>
