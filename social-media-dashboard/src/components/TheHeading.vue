<template>
  <header class="header">
    <div class="container--header">
      <div class="container--title">
        <div class="header--title">{{ titulo }}</div>
        <h3 class="header--subtitle">{{ subtitulo }}</h3>
      </div>
      <div class="container--toggle">
        <div class="toggle--text">
          <h3>Dark mode</h3>
        </div>
        <div class="toggle--checkbox">
          <label class="toggle">
            <input
              type="checkbox"
              checked
              v-model="stateCheckbox"
              v-on:click="cambiaTema()"
            />
            <span class="slider"></span>
          </label>
        </div>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  name: "TheHeading",
  props: {
    titulo: String,
    subtitulo: String,
  },

  data() {
    return {
      stateCheckbox: "true",
    };
  },

  methods: {
    cambiaTema: function () {
      if (this.stateCheckbox) {
        document.documentElement.setAttribute("modo-oscuro", "activado");
      } else {
        document.documentElement.setAttribute("modo-oscuro", "desactivado");
      }
    },
  },
};
</script>