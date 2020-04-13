<template>
  <div id="page-content">
    <TempVarChart :tempVar="weatherData.temperature" />
    <Highlights :highlights="weatherData.highlights" />
  </div>
</template>

<script>
import TempVarChart from "@/components/TempVarChart.vue";
import Highlights from "@/components/Highlights.vue";

export default {
  name: "Content",
  components: {
    TempVarChart,
    Highlights
  },
  props: {
    weatherData: {
      type: Object
    }
  }
};
</script>

<style lang="scss" scoped>
#page-content {
  border: 1px solid black;
  padding: 2px;
}
</style>
