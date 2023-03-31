<script>
export default {
  data() {
    return {
      pokemons: [
        {
          name: 'q232214235',
          url: 'https://assets.pokemon.com/assets/cms2/img/pokedex/detail/010.png'
        },
        {
          name: '2',
          url: 'https://assets.pokemon.com/assets/cms2/img/pokedex/detail/010.png'
        },
        {
          name: '3',
          url: 'https://assets.pokemon.com/assets/cms2/img/pokedex/detail/010.png'
        },
        {
          name: '4',
          url: 'https://assets.pokemon.com/assets/cms2/img/pokedex/detail/010.png'
        },
        {
          name: '5',
          url: 'https://assets.pokemon.com/assets/cms2/img/pokedex/detail/010.png'
        },
        {
          name: '6',
          url: 'https://assets.pokemon.com/assets/cms2/img/pokedex/detail/010.png'
        },
        {
          name: '7',
          url: 'https://assets.pokemon.com/assets/cms2/img/pokedex/detail/010.png'
        },
        {
          name: '8',
          url: 'https://assets.pokemon.com/assets/cms2/img/pokedex/detail/010.png'
        },
        {
          name: '9',
          url: 'https://assets.pokemon.com/assets/cms2/img/pokedex/detail/010.png'
        },
        {
          name: '10',
          url: 'https://assets.pokemon.com/assets/cms2/img/pokedex/detail/010.png'
        },
        {
          name: '11',
          url: 'https://assets.pokemon.com/assets/cms2/img/pokedex/detail/010.png'
        },
        {
          name: '12',
          url: 'https://assets.pokemon.com/assets/cms2/img/pokedex/detail/010.png'
        }
      ]
    }
  }
}
</script>
<style>
h1 {
  text-align: center;
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
  width: 65px;
  height: 65px;
  margin-left: 5px;
}
.image {
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
<template>
  <body>
    <h1>Build Your Team</h1>
    <div class="Mons">
      <div class="card" v-for="pokemon in pokemons">
        <p class="pokename">{{ pokemon.name }}</p>
        <div class="image"><img :src="pokemon.url" /></div>
        <button class="addTeam">
          <p>ADD TO TEAM</p>
        </button>
      </div>
    </div>
  </body>
</template>
<!-- data() { return { items: [{ message: 'Foo' },{ message: 'Bar' }] } } template
<li v-for="item in items">
  {{ item.message }}
</li> -->
