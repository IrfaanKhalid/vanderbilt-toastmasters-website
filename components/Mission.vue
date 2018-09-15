<template>
  <section class="container">
    <div class="mission">
      <div class="mission-statement title">
        To craft our members' communication and leadership skills in a mutually supportive and positive learning environment.
      </div>
      <div class="mission-description subtitle">
        Via regular meetings and external mentorship, our members strive to grow every day as leaders and communicators.
      </div>
    </div>
  </section>
</template>

<style lang="css" scoped>
.mission {
  min-height: 100vh;
  max-height: 100vh;
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
  box-shadow: 5px 5px 5px black;
  min-height: 50vh;
  justify-content: center;
}

.mission-description {
  grid-area: description;
  justify-content: center;
  text-align: center;
  margin-left: 5vw;
  margin-right: 5vw;
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
