<template>
  <div class="container">
    <the-header title="Study App"></the-header>
    <stored-data :data-p="storedData"> </stored-data>
  </div>
</template>

<script>
  import TheHeader from "./components/layout/TheHeader.vue";

import StoredData from "./components/learning-data/StoredData.vue";

export default {
  name: "App",
  components: {
    StoredData,
    TheHeader
  },
  data() {
    return {
      storedData: [
        {
          id: 1,
          title: "VueJs",
          description: "Vue Js Styleguide and Allgemeines",
          link: "https://vuejs.org",
        },
        {
          id: 2,
          title: "PHP",
          description: "PHP Guide",
          link: "https://php.net/",
        },
      ],
    };
  },
};
</script>

<style>
  body{
    box-sizing: border-box;
    margin: 0;
    padding: 0;
  }
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;


}
</style>
