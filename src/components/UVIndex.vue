<template>
  <div id="uv-index">
    <p>UV Index: {{ uvIndex }}</p>
  </div>
</template>

<script>
export default {
  name: "UVIndex",
  props: {
    uvIndex: {
      type: Number
    }
  }
};
</script>
