<template>
  <div class="card">
    <div class="card--header">
      <figure
        class="icon-here"
        :fondo-icon="fondoIcon"
        id="redSocialIcon"
      ></figure>
      <span class="card--header-title">{{ nombre }} </span>
    </div>
    <div class="padd-30b">
      <div class="card--number">{{ numeroSeguidores }}</div>
      <div class="card--follows">{{ textoSeguidores }}</div>
    </div>
    <div class="card--footer">
      <figure class="icon-row" :flecha-icon="flechaIcon"></figure>
      <span class="card--footer-content" :color-texto="flechaIcon">{{
        textoActuales
      }}</span>
    </div>
  </div>
</template>

<script>
export default {
  name: "BaseCardMain",
  props: {
    nombre: String,
    numeroSeguidores: String,
    textoSeguidores: String,
    textoActuales: String,
    fondoIcon: String,
    flechaIcon: String,
  },

  mounted: function () {
    this.cargaLogosCards();
    this.flechaLogoCards();
  },

  methods: {
    cargaLogosCards: function () {
      switch (this.fondoIcon) {
        case "Facebook":
          document.documentElement.setAttribute("fondo-icon", "Facebook");
          break;

        case "Twitter":
          document.documentElement.setAttribute("fondo-icon", "Twitter");
          break;

        case "Instagram":
          document.documentElement.setAttribute("fondo-icon", "Instagram");
          break;

        case "Youtube":
          document.documentElement.setAttribute("fondo-icon", "Youtube");
          break;

        default:
          document.documentElement.setAttribute("fondo-icon", "Twitter");
          break;
      }
    },
    flechaLogoCards: function () {
      switch (this.flechaIcon) {
        case "Up":
          document.documentElement.setAttribute("flecha-icon", "Up");
          document.documentElement.setAttribute("color-texto", "Up");
          break;

        case "Down":
          document.documentElement.setAttribute("flecha-icon", "Down");
          document.documentElement.setAttribute("color-texto", "Down");
          break;

        default:
          document.documentElement.setAttribute("flecha-icon", "Up");
          break;
      }
    },
  },
};
</script>