<template>
  <div class="pokemon-list-item">
    <li v-on:click="handleClick">{{ pokemon.name }}</li>
  </div>
</template>

<script>
import { eventBus } from "../main";
export default {
  name: "PokemonListItem",
  props: ["pokemon"],
  methods: {
    handleClick: function () {
      eventBus.$emit('pokemon-selected', this.pokemon);
    },
  },
};
</script>

<style>
</style>