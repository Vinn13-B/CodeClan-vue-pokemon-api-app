<template>
  <div id="pokemon-list">
    <h2>Pokemon List</h2>
    <ul>
      <pokemon-list-item
        v-for="(pokemon, index) in allPokemon"
        :key="index"
        :pokemon="pokemon"
      ></pokemon-list-item>
    </ul>
  </div>
</template>

<script>
import PokemonListItem from "./PokemonListItem.vue";
export default {
  name: "PokemonList",
  props: ["allPokemon"],
  components: {
    "pokemon-list-item": PokemonListItem,
  },
};
</script>

<style>
</style>