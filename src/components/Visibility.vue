<template>
  <div id="visibility">
    <p>Visibility: {{ visibility }}</p>
  </div>
</template>

<script>
export default {
  name: "Visibility",
  props: {
    visibility: {
      type: String
    }
  }
};
</script>
