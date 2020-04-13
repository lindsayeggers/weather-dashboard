<template>
  <div id="wind-status">
    <p>Wind Speed: {{ windStatus.speed }}</p>
    <p>
      Wind Direction - {{ windStatus.derivedWindDirection }} or
      {{ windStatus.direction }}
    </p>
  </div>
</template>

<script>
export default {
  name: "windStatus",
  props: {
    windStatus: {
      type: Object
    }
  }
};
</script>
