<template>
  <div id="app">
      <app-header :projectTitle="projectTitle"></app-header>
      <app-main></app-main>
      <app-footer :cert="cert" :project="project"></app-footer>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Main from "./components/Main.vue";
import Footer from "./components/Footer.vue";

const PROJECT_TITLE = "Local Weather";
const CERT = "frontend";
const PROJECT = "local-weather";

export default {
  name: "app",
  components: {
      "app-header": Header,
      "app-main": Main,
      "app-footer": Footer
  },
  data() {
        return {
            projectTitle: PROJECT_TITLE,
            cert: CERT,
            project: PROJECT
        };
    }
}
</script>

<style>
@import "./assets/scss/style";
</style>
