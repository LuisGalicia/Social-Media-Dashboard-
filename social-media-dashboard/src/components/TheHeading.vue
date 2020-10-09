<template>
  <header class="header">
    <div class="container">
      <h1 class="header--title">{{ titulo }}</h1>
      <h3 class="header--subtitle">{{ subtitulo }}</h3>
    </div>
    <div class="container--toggle">
      <div class="toggle--text">
        <h3>Dark mode</h3>
      </div>
      <div class="toggle--checkbox">
          <label class=" toggle">
              <input type="checkbox" checked>
              <span class="slider"></span>
          </label>
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
};
</script>