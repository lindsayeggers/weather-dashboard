<template>
  <div id="temp">
    {{ tempVar.tempToday }}
  </div>
</template>

<script>
export default {
  name: "TempVarChart",
  props: {
    tempVar: {
      type: Object
    }
  }
};
</script>
