


<template>
    <div>
 <h1>Choose Pokemon</h1>  
  <div class="Mons">
      <div class="card" v-for="pokemon in pokemons"
        :key="pokemon.name">
        <p class="pokename">{{ pokemon.name }}</p>
        <div class="image"><img :src="pokemon.url" /></div>
        <button v-on:click="addItemToCart(pokemon)" class="addTeam">
         <h2>+</h2>
        </button>
      </div>
    </div> 
</div>
</template>

<script>
export default {}

</script>

<style></style>



