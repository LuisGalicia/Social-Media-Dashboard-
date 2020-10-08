<template>
  <div>
    <div>
      <p>{{ overviewTextoCarta }}</p>
    </div>
    <div>
      <p>{{ overviewTotalVistas }}</p>
    </div>
    <div>
      <p>{{ overviewPorcentajeVistas }}</p>
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
  },
};
</script>