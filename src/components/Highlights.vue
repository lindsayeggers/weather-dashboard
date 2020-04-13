<template>
  <div id="highlights">
    <UVIndex :uvindex="highlights.uvindex" />
    <Visibility :visibility="highlights.visibility" />
    <WindStatus :windStatus="highlights.windstatus" />
  </div>
</template>

<script>
import UVIndex from "@/components/UVIndex.vue";
import Visibility from "@/components/Visibility.vue";
import WindStatus from "@/components/WindStatus.vue";

export default {
  name: "Highlights",
  components: {
    UVIndex,
    Visibility,
    WindStatus
  },
  props: {
    highlights: {
      type: Object
    }
  }
};
</script>
