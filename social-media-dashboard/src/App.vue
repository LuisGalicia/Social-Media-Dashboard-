<template>
  <div id="app">
    <TheHeading
      titulo="Social Media Dashboard"
      subtitulo="Total Followers: 23,004"
    />
    <BaseCardMain
      nombre="@nathanf"
      numeroSeguidores="1987"
      textoSeguidores="Followers"
      textoActuales="12 Today"
    />
    <TheSubtitle titulo="Overview" />
    <BaseCardOverview
      overviewTextoCarta="Page Views"
      overviewTotalVistas="87"
      overviewPorcentajeVistas="3%"
    />
  </div>
</template>

<script>
import TheHeading from "./components/TheHeading.vue";
import TheSubtitle from "./components/TheSubtitle.vue";
import BaseCardMain from "./components/BaseCardMain.vue";
import BaseCardOverview from "./components/BaseCardOverview.vue";

export default {
  name: "App",
  components: {
    TheHeading,
    TheSubtitle,
    BaseCardMain,
    BaseCardOverview,
  },
};
</script>

