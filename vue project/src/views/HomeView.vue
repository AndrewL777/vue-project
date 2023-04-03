<<<<<<< HEAD
<template>

  <header> <button v-on:click="navigateTo('Pokemon You Chose')"  > View Team </button>
    <button v-on:click="navigateTo('Pick Your Pokemon')"  > Choose Team </button> </header>

{{ page }}
  <div v-if="page === 'Pokemon You Chose'">  
<h1>Your Team</h1>
<div class="Mons">
    <div class="card" v-for="pokemon in team"
      :key="pokemon.name">
      <p class="pokename">{{ pokemon.name }}</p>
      <div class="image"><img :src="pokemon.url" /></div>
      <button v-on:click="RemovePokemonFromTeam(pokemon)" class="addTeam">
       <h2>-</h2>
      </button>
    </div>
  </div> </div>    


<div v-if="page==='Pick Your Pokemon'"> 
=======



<template>
  <div>
>>>>>>> parent of 0237d6a (2)
<h1>Choose Pokemon</h1>  
<div class="Mons">
    <div class="card" v-for="pokemon in pokemons"
      :key="pokemon.name">
      <p class="pokename">{{ pokemon.name }}</p>
      <div class="image"><img :src="pokemon.url" /></div>
<<<<<<< HEAD
      <button v-on:click="addItemToTeam(pokemon)" class="addTeam">
=======
      <button v-on:click="addItemToCart(pokemon)" class="addTeam">
>>>>>>> parent of 0237d6a (2)
       <h2>+</h2>
      </button>
    </div>
  </div> 
</div>
<<<<<<< HEAD

</template>
<script>



export default {
name:"pokes",
data() {
  return {
    page: "Pick Your Pokemon",
    team: [],
    pokemons: [
      {
        name: 'Lugia',
        url: 'https://assets.pokemon.com/assets/cms2/img/pokedex/detail/249.png'
      },
      {
        name: 'Articuno',
        url: 'https://assets.pokemon.com/assets/cms2/img/pokedex/detail/144.png'
      },
      {
        name: 'Tinkaton',
        url: 'https://assets.pokemon.com/assets/cms2/img/pokedex/detail/959.png'
      },
      {
        name: 'Hydreigon',
        url: 'https://assets.pokemon.com/assets/cms2/img/pokedex/detail/635.png'
      },
      {
        name: 'Ceruledge',
        url: 'https://assets.pokemon.com/assets/cms2/img/pokedex/detail/937.png'
      },
      {
        name: 'Sandy Shocks',
        url: 'https://assets.pokemon.com/assets/cms2/img/pokedex/detail/989.png'
      },
      {
        name: 'Koraidon',
        url: 'https://assets.pokemon.com/assets/cms2/img/pokedex/detail/1007.png'
      },
      {
        name: 'Rayquaza',
        url: 'https://assets.pokemon.com/assets/cms2/img/pokedex/detail/384.png'
      },
      {
        name: 'Charizard',
        url: 'https://assets.pokemon.com/assets/cms2/img/pokedex/detail/006.png'
      },
      {
        name: 'Guzzlord',
        url: 'https://assets.pokemon.com/assets/cms2/img/pokedex/detail/799.png'
      },
      {
        name: 'Mewtwo',
        url: 'https://assets.pokemon.com/assets/cms2/img/pokedex/detail/150.png'
      },
      {
        name: 'Garchomp',
        url: 'https://assets.pokemon.com/assets/cms2/img/pokedex/detail/445.png'
      },
      {
        name: 'Lucario',
        url: 'https://assets.pokemon.com/assets/cms2/img/pokedex/detail/448.png'
      },
      {
        name: 'Dragonite',
        url: 'https://assets.pokemon.com/assets/cms2/img/pokedex/detail/149.png'
      },
      {
        name: 'Suicune',
        url: 'https://assets.pokemon.com/assets/cms2/img/pokedex/detail/245.png'
      },
      {
        name: 'Jolteon',
        url: 'https://assets.pokemon.com/assets/cms2/img/pokedex/detail/135.png'
      },
      {
        name: 'Salamance',
        url: 'https://assets.pokemon.com/assets/cms2/img/pokedex/detail/373.png'
      },
      {
        name: 'Kingambit',
        url: 'https://assets.pokemon.com/assets/cms2/img/pokedex/detail/983.png'
      },
      {
        name: 'Accelgor',
        url: 'https://assets.pokemon.com/assets/cms2/img/pokedex/detail/617.png'
      },
      {
        name: 'Darkrai',
        url: 'https://assets.pokemon.com/assets/cms2/img/pokedex/detail/491.png'
      },
      {
        name: 'Kyogre',
        url: 'https://assets.pokemon.com/assets/cms2/img/pokedex/detail/382.png'
      },
      {
        name: 'Kingdra',
        url: 'https://assets.pokemon.com/assets/cms2/img/pokedex/detail/230.png'
      },
      {
        name: 'Blastoise',
        url: 'https://assets.pokemon.com/assets/cms2/img/pokedex/detail/009.png'
      },
      {
        name: 'Pikachu',
        url: 'https://assets.pokemon.com/assets/cms2/img/pokedex/detail/025.png'
      }
   
     

    ]
  }
},
methods: {
  addItemToTeam(pokemon){
    this.team.push(pokemon);
    console.log(this.team)
  },
  navigateTo(page) {
    this.page = page;
  },
  RemovePokemonFromTeam(pokemon){
    this.team.splice(this.team.indexOf(pokemon));
  }
}
}
</script>
<style>
h1 {
text-align: center;
}
h2 {
font-size: 10px;

}
p{
text-align: center;
font-size: 20px;
}
.Mons {
margin-top: 100px;
display: flex;
flex-direction: row;
flex-wrap: wrap;
justify-content: space-between;
}
.card {
width: 300px;
height: 300px;
margin-top: 40px;
border: 3px solid black;
}

.addTeam {
width: 30px;
height: 30px;
margin-left: 5px;
}
.image {
width: 20px;
margin-left: 40px;
}
.pokename {
margin: auto;
width: 50%;
margin-top: 3px;
border: 3px solid black;
padding: 10px;
}
</style>
<!-- make placeholders, use absolute positioning with ref,  -->

<!-- data() { return { items: [{ message: 'Foo' },{ message: 'Bar' }] } } template
<li v-for="item in items">
{{ item.message }}
</li> -->
=======
</template>

<script>
export default {}

</script>

<style></style>



>>>>>>> parent of 0237d6a (2)
