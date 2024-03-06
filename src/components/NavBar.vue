<template>
  <v-app-bar
    app
    color="black"
    dark
    flat
    class="px-12"
    style="position: fixed; top: 0"
  >
    <v-btn text @click="scroll('home')">Home</v-btn>
    <v-btn text @click="scroll('about')">About</v-btn>
    <v-btn text @click="scroll('portfolio')">Projects</v-btn>
    <v-btn text @click="scroll('skills')"> Skills</v-btn>
    <v-btn text @click="scroll('contact')"> Contact</v-btn>
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

<style></style>
