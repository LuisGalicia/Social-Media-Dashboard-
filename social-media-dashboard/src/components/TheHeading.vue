<template>
  <header class="container__header">
    <div class="header">
      <div class="header__header">
        <div class="header__title">{{ titulo }}</div>
        <h3 class="header__subtitle">{{ subtitulo }}</h3>
      </div>
      <div class="header__toggle">
        <div class="header__toggle-text">
          <h3>Dark mode</h3>
        </div>
        <div class="header__toggle-container">
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