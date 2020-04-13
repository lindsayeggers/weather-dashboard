<template>
  <div id="app">
    <p>This component's code is in {{ filename }}'</p>
    <Content :weatherData="weatherData" />
  </div>
</template>

<script>
import Content from "@/components/Content.vue";

export default {
  components: {
    Content
  },
  data() {
    return {
      filename: "App.vue",
      weatherData: {
        location: "California",
        temperature: {
          current: "35 C"
        },
        highlights: {
          uvindex: "3",
          windstatus: {
            speed: "20 km/h",
            direction: "N-E"
          },
          visibility: "12 km"
        }
      }
    };
  }
};
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
