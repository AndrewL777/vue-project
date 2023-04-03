<<<<<<< HEAD
<script setup>
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
=======
<template>

    <header> <button v-on:click="navigateTo('cart')"  > View Team </button>
      <button v-on:click="navigateTo('products')"  > Choose Team </button> </header>
 
 {{ page }}
    <div v-if="page === 'cart'">  
  <h1>Your Team</h1>
  <div class="Mons">
      <div class="card" v-for="pokemon in cart"
        :key="pokemon.name">
        <p class="pokename">{{ pokemon.name }}</p>
        <div class="image"><img :src="pokemon.url" /></div>
        <button v-on:click="RemoveItemFromCart(pokemon)" class="addTeam">
         <h2>-</h2>
        </button>
      </div>
    </div> 
  </div>    


<div v-if="page==='products'"> 
  <Mons />
  
  </div>

</template>


<script>
import Mons from  './views/ChooseThings.Vue';
export default {
  name:"pokes",
  data() {
    return {
      page: "products",
      cart: [],
      pokemons: [
        {
          name: 'Lugia',
          url: 'https://assets.pokemon.com/assets/cms2/img/pokedex/detail/249.png'
        },
        {
          name: 'Drowzee',
          url: 'https://assets.pokemon.com/assets/cms2/img/pokedex/detail/096.png'
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
        }
      ]
    }
  },
  methods: {
    addItemToCart(pokemon){
      this.cart.push(pokemon);
      console.log(this.cart)
    },
    navigateTo(page) {
      this.page = page;
    },
    RemoveItemFromCart(pokemon){
      this.cart.splice(this.cart.indexOf(pokemon));
    }
  }
}
>>>>>>> parent of 0237d6a (2)
</script>

<template>
  <header>
    <img alt="Vue logo" class="logo" src="@/assets/logo.svg" width="125" height="125" />

<<<<<<< HEAD
    <div class="wrapper">
      <HelloWorld msg="hi!" />

      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
      </nav>
    </div>
  </header>

  <RouterView />
</template>
=======
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
>>>>>>> parent of 0237d6a (2)
