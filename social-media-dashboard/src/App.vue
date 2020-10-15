<template>
  <div id="app">
    <TheHeading
      titulo="Social Media Dashboard"
      subtitulo="Total Followers: 23,004"
    />
    <div class="container">
      <div class="container--socialNetwork">
        <BaseCardMain
        nombre="@nathanf"
        numeroSeguidores="1987"
        textoSeguidores="Followers"
        textoActuales="12 Today"
      />
      <BaseCardMain
        nombre="@nathanf"
        numeroSeguidores="1044"
        textoSeguidores="Followers"
        textoActuales="99 Today"
      />
      <BaseCardMain
        nombre="@realnathanf"
        numeroSeguidores="11k"
        textoSeguidores="Followers"
        textoActuales="1099 Today"
      />
      <BaseCardMain
        nombre="Nathan F."
        numeroSeguidores="8239"
        textoSeguidores="Subscribers"
        textoActuales="144 Today"
      />
      </div>
      
      <TheSubtitle titulo="Overview" />
      <BaseCardOverview
        overviewTextoCarta="Page Views"
        overviewTotalVistas="87"
        overviewPorcentajeVistas="3%"
      />
    </div>
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

