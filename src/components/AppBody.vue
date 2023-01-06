<template>
  <div class="container">
    <SoundButton
      v-for="sound in this.sounds"
      :key="sound.name"
      :sound="sound"
    />
  </div>
</template>

<script>
import SoundButton from "./SoundButton.vue";

export default {
  name: "AppBody",
  components: {
    SoundButton,
  },
  props: ["sounds"],
};
</script>

<style scoped>
.container {
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
  gap: 20px;
}
</style>
