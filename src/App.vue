<script>
import Header from "./components/Header.vue";
import Main from "./components/Main.vue";
import { store } from "./store";
export default {
  data() {
    return {
      store: store,
    };
  },

  components: {
    Header,
    Main,
  },

  methods: {},

  mounted() {
    // console.log(this.store)
  },
};
</script>

<template>
  <Header />
  <Main />
</template>

<style>
@import "bootstrap/dist/css/bootstrap.min.css";
</style>
