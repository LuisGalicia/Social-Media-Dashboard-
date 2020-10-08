<template>
  <div>
    <div>{{ nombre }}</div>
    <div>
      <p>{{ numeroSeguidores }}</p>
      <p>{{ textoSeguidores }}</p>
    </div>
    <div>{{ textoActuales }}</div>
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