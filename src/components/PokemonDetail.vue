<template>
  <div id="pokemon-detail">
    <h2>{{ pokemon.name.toUpperCase() }}</h2>
    <img :src="pokemon.sprites.other.dream_world.front_default" />
  </div>
</template>

<script>
export default {
  name: "PokemonDetail",
  props: ["pokemon"],
};
</script>

<style>
</style>