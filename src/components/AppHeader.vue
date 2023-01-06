<template>
  <div class="conteiner">
    <h1>Szkolna 17 dictionary</h1>
  </div>
</template>

<script>
export default {
  name: "AppHeader",

  data() {
    return {
      menuElements: [
        { name: "Start", id: "start" },
        { name: "Projects", id: "projects" },
        { name: "Contact", id: "contact" },
      ],
      displayMenu: true,
      isMobile: true,
    };
  },
  methods: {},
};
</script>
<style scoped>
h1 {
  text-align: center;
  padding: 20px;
}
</style>
