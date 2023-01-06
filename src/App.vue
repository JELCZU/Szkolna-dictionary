<template>
  <div>
    <AppHeader />
    <AppBody :sounds="sounds" />
    <AppFooter />
  </div>
</template>

<script>
import AppHeader from "./components/AppHeader.vue";
import AppBody from "./components/AppBody.vue";
import AppFooter from "./components/AppFooter.vue";

export default {
  name: "App",
  components: {
    AppHeader,
    AppBody,
    AppFooter,
  },
  data() {
    return {
      sounds: [
        {
          name: "Bitwa pod grunwaldem",
          src: "Bitwa-pod-Grunwaldem.mp3",
        },
        {
          name: "Chcesz mieć problem?",
          src: "Chcesz-miec-problem.mp3",
        },
        {
          name: "Do Choroszczy na badania",
          src: "Do-Choroszczy-na-badania.mp3",
        },
        {
          name: "Do Choroszczy niedługo pojedziesz",
          src: "Do-Choroszczy-niedlugo-pojedziesz.mp3",
        },
        {
          name: "Już pół słoika opier...",
          src: "Juz-pol-sloika-opier.mp3",
        },
        {
          name: "Kto zatrzymał ziemię",
          src: "Kto-zatrzymal-ziemie.mp3",
        },
        {
          name: "Ludzki miód",
          src: "Ludzki-miod.mp3",
        },
        {
          name: "Muszę mieć lepszą wiadomość",
          src: "Musze-miec-lepsza-wiadomosc.mp3",
        },
        {
          name: "Nie bierz mojej kiełbasy",
          src: "Nie-bierz-mojej-kielbasy.mp3",
        },
        {
          name: "O cholera",
          src: "O-cholera.mp3",
        },
        {
          name: "Pachnie dupa",
          src: "Pachnie-dupa.mp3",
        },
        {
          name: "Prosze sie nie odzywać",
          src: "Prosze-sie-nie-odzywac.mp3",
        },
        {
          name: "Przegiąłeś pałę",
          src: "Przegieles-pale.mp3",
        },
      ],
    };
  },
};
</script>

<style>
* {
  box-sizing: border-box;
  font-family: Open Sans, sans-serif;
}
:root {
  --dark-color: #181818;
  --darker-color: #1f1f1f;
  --lighter-color: #252525;
  --light-color: #3c3c3c;
  background-color: var(--light-color);
}
body {
  padding: 0;
  margin: 0;
}
button {
  cursor: pointer;
}
.container {
  padding: 50px 20px;
}

h1,
h2,
h3,
h4,
li {
  color: #ffffff;
  padding: 0;
  margin: 0;
}
h1 {
  font-size: 32px;
}
h2 {
  font-size: 18px;
}
/* h3 {
  font-size: 18px;
} */
</style>
