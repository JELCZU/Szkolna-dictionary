<template>
  <button @click="this.playSound()">
    <h2>{{ this.sound.name }}</h2>
  </button>
</template>

<script>
export default {
  name: "SoundButton",

  props: ["sound"],
  data() {
    return {
      audio: null,
    };
  },
  methods: {
    playSound() {
      this.audio.play();
    },
  },
  mounted() {
    // eslint-disable-next-line global-require, import/no-unresolved, import/no-dynamic-require
    this.audio = new Audio(require(`@/assets/sound/${this.sound.src}`));
  },
};
</script>

<style scoped>
button {
  background-color: var(--lighter-color);
  border-style: none;
  padding: 20px;
  width: 300px;
  height: 80px;
  /* max-width: 30vw; */
}
button:hover {
  background-color: var(--dark-color);
}
</style>
