<template>
  <div class="card">
    <h3 class="card--title">{{ nombre }}</h3>
    <div class="container--cardNumber">
      <div class="card--number">{{ numeroSeguidores }}</div>
      <div class="card--follows">{{ textoSeguidores }}</div>
    </div>
    <div class="card--today-up">{{ textoActuales }}</div>
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
  },
 
};
</script>