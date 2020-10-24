<template>
  <div id="app">
    <TheHeading
      titulo="Social Media Dashboard"
      subtitulo="Total Followers: 23,004"
    />
    <div class="container">
      <div class="container--grid-primary">
        <BaseCardMain
          nombre="@nathanf"
          numeroSeguidores="1987"
          textoSeguidores="Followers"
          textoActuales="12 Today"
          fondoIcon="Facebook"
          flechaIcon="Up"
        />
        <BaseCardMain
          nombre="@nathanf"
          numeroSeguidores="1044"
          textoSeguidores="Followers"
          textoActuales="99 Today"
          fondoIcon="Twitter"
          flechaIcon="Up"
        />
        <BaseCardMain
          nombre="@realnathanf"
          numeroSeguidores="11k"
          textoSeguidores="Followers"
          textoActuales="1099 Today"
          fondoIcon="Instagram"
          flechaIcon="Up"
        />
        <BaseCardMain
          nombre="Nathan F."
          numeroSeguidores="8239"
          textoSeguidores="Subscribers"
          textoActuales="144 Today"
          fondoIcon="Youtube"
          flechaIcon="Down"
        />
      </div>

      <TheSubtitle titulo="Overview today" />

      <div class="container--grid-primary">
        <BaseCardOverview
          overviewTextoCarta="Page Views"
          overviewTotalVistas="87"
          overviewPorcentajeVistas="3%"
          overviewLogo="Facebook"
          rowIcon="Up"
        />
        <BaseCardOverview
          overviewTextoCarta="Likes"
          overviewTotalVistas="52"
          overviewPorcentajeVistas="2%"
          overviewLogo="Facebook"
          rowIcon="Down"
        />
        <BaseCardOverview
          overviewTextoCarta="Likes"
          overviewTotalVistas="5462"
          overviewPorcentajeVistas="2257%"
          overviewLogo="Instagram"
          rowIcon="Up"
        />
        <BaseCardOverview
          overviewTextoCarta="Profile Views"
          overviewTotalVistas="52k"
          overviewPorcentajeVistas="1375%"
          overviewLogo="Instagram"
          rowIcon="Up"
        />
      </div>

      <div class="container--grid-primary padd-25t">
        <BaseCardOverview
          overviewTextoCarta="Retweets"
          overviewTotalVistas="117"
          overviewPorcentajeVistas="303%"
          overviewLogo="Twitter"
          rowIcon="Up"
        />
        <BaseCardOverview
          overviewTextoCarta="Likes"
          overviewTotalVistas="507"
          overviewPorcentajeVistas="553%"
          overviewLogo="Twitter"
          rowIcon="Up"
        />
        <BaseCardOverview
          overviewTextoCarta="Likes"
          overviewTotalVistas="107"
          overviewPorcentajeVistas="19%"
          overviewLogo="Youtube"
          rowIcon="Down"
        />
        <BaseCardOverview
          overviewTextoCarta="Total Views"
          overviewTotalVistas="1407"
          overviewPorcentajeVistas="12%"
          overviewLogo="Youtube"
          rowIcon="Down"
        />
      </div>
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

