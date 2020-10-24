<template>
  <div class="card--overview">
    <div class="container--grid-secundary">
      <div class="card--overview--title">
        {{ overviewTextoCarta }}
      </div>
      <div class="card--overview--icon">
        <figure class="icon-here" :overview-logo="overviewLogo"></figure>
      </div>
    </div>
    <div class="container--grid-secundary">
      <div class="card--overview--number">
        {{ overviewTotalVistas }}
      </div>
      <div class="card--overview--footer">
        <figure class="icon-row" :overview-row-icon="rowIcon"></figure>
        <span
          class="card--overview--footer-content"
          :overview-text-color="rowIcon"
          >{{ overviewPorcentajeVistas }}</span
        >
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "BaseCardOverview",
  props: {
    overviewTextoCarta: String,
    overviewTotalVistas: String,
    overviewPorcentajeVistas: String,
    overviewLogo: String,
    rowIcon: String,
  },

  mouted: function () {
    this.cargaLogosOverviewCard();
    this.cargaFlechaColor();
  },

  methods: {
    cargaLogosOverviewCard: function () {
      switch (this.overviewLogo) {
        case "Facebook":
          document.documentElement.setAttribute("overview-logo", "Facebook");
          break;
        case "Twitter":
          document.documentElement.setAttribute("overview-logo", "Twitter");
          break;
        case "Instagram":
          document.documentElement.setAttribute("overview-logo", "Instagram");
          break;
        case "Youtube":
          document.documentElement.setAttribute("overview-logo", "Youtube");
          break;
        default:
          document.documentElement.setAttribute("overview-logo", "Twitter");
          break;
      }
    },

    cargaFlechaColor: function () {
      switch (this.rowIcon) {
        case "Up":
          document.documentElement.setAttribute("overview-row-icon", "Up");
          document.documentElement.setAttribute("overview-text-color", "Up");
          break;
        case "Down":
          document.documentElement.setAttribute("overview-row-icon", "Down");
          document.documentElement.setAttribute("overview-text-color", "Down");
          break;
        default:
          break;
      }
    },
  },
};
</script>