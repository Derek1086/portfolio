<template>
  <v-app-bar
    app
    color="black"
    dark
    flat
    style="position: fixed; top: 0"
    class="main-bar"
  >
    <div class="spacer" />
    <v-btn text size="small" @click="scroll('home')" class="nav-btn"
      >Home</v-btn
    >
    <v-btn text size="small" @click="scroll('about')" class="nav-btn"
      >About</v-btn
    >
    <v-btn text size="small" @click="scroll('portfolio')" class="nav-btn"
      >Projects</v-btn
    >
    <v-btn text size="small" @click="scroll('skills')" class="nav-btn">
      Skills</v-btn
    >
    <v-btn text size="small" @click="scroll('contact')" class="nav-btn">
      Contact</v-btn
    >
  </v-app-bar>
</template>

<script>
export default {
  methods: {
    scroll(refName) {
      const element = document.getElementById(refName);
      element.scrollIntoView({ behavior: "smooth" });
    },
  },
};
</script>

<style scoped>
.spacer {
  margin-left: 5%;
}

.main-bar {
  width: 100%;
  height: 10vh;
  background-color: black;
  color: white;
}

.nav-btn {
  transition: color 0.5s, text-decoration 0.5s;
  border-radius: 0px !important;
  font-size: 1rem;
  height: 100% !important;
}

.nav-btn:hover {
  color: grey !important;
  border-bottom: 2px solid grey !important;
}

@media only screen and (max-width: 600px) {
  .spacer {
    margin-left: 8%;
  }

  .nav-btn {
    font-size: 0.55rem;
  }
}
</style>
