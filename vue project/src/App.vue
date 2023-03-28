<script>
export default {
  data() {
    return {
      pokemons: [
        {
          name: 'Char',
          url: ''
        },
        {
          name: '2',
          url: ''
        },
        {
          name: '3',
          url: ''
        },
        {
          name: '4',
          url: ''
        },
        {
          name: '5',
          url: ''
        },
        {
          name: '6',
          url: ''
        },
        {
          name: '7',
          url: ''
        },
        {
          name: '8',
          url: ''
        },
        {
          name: '9',
          url: ''
        },
        {
          name: '10',
          url: ''
        },
        {
          name: '11',
          url: ''
        },
        {
          name: '12',
          url: ''
        }
      ]
    }
  }
}
</script>
<style>
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
  box-shadow: 1px 1px 1px;
}
.addTeam {
  width: 65px;
  height: 65px;
  margin-left: 5px;
}
.pokename {
  margin: auto;
  width: 50%;
  margin-top: 1px;
  border: 1px solid black;
  padding: 10px;
}
</style>
<!-- make placeholders  -->
<template>
  <body>
    <h1>21</h1>
    <div class="Mons">
      <div class="card" v-for="pokemon in pokemons">
        <p class="pokename">{{ pokemon.name }}</p>

        <button class="addTeam">
          <p>ADD TO TEAM</p>
          <img :src="pokemon.url" />
        </button>
      </div>
    </div>
  </body>
</template>
<!-- data() { return { items: [{ message: 'Foo' },{ message: 'Bar' }] } } template
<li v-for="item in items">
  {{ item.message }}
</li> -->
