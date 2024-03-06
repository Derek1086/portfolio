<template>
  <v-app-bar
    app
    color="black"
    dark
    flat
    class="px-12"
    style="position: fixed; top: 0"
  >
    <v-btn text @click="scroll('home')" class="nav-btn">Home</v-btn>
    <v-btn text @click="scroll('about')" class="nav-btn">About</v-btn>
    <v-btn text @click="scroll('portfolio')" class="nav-btn">Projects</v-btn>
    <v-btn text @click="scroll('skills')" class="nav-btn"> Skills</v-btn>
    <v-btn text @click="scroll('contact')" class="nav-btn"> Contact</v-btn>
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
.nav-btn {
  transition: color 0.5s, text-decoration 0.5s;
  border-radius: 0px !important;
}

.nav-btn:hover {
  color: grey !important;
  border-bottom: 2px solid grey !important;
}
</style>
