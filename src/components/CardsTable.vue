<template>
  <div>
    <card v-for="card in $store.state.table" :key="card.id" :id="card.id" />
  </div>
  <!-- agragr un boton de play al que le tengo que asociar el estado para que se muetre cuando este activado (select cartad e iniciar juego) -->
</template>

<script>
import Card from "./Card.vue";

export default {
  components: {
    Card
  }
}
</script>

<style scoped lang="scss">
div {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
}
</style>
