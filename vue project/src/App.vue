<script>
export default {
  data() {
    return {
      pokemons: [
        {
          name: '',
          url: ''
        },
        {
          name: '',
          url: ''
        },
        {
          name: '',
          url: ''
        },
        {
          name: '',
          url: ''
        },
        {
          name: '',
          url: ''
        },
        {
          name: '',
          url: ''
        },
        {
          name: '',
          url: ''
        },
        {
          name: '',
          url: ''
        },
        {
          name: '',
          url: ''
        },
        {
          name: '',
          url: ''
        },
        {
          name: '',
          url: ''
        },
        {
          name: '',
          url: ''
        }
      ]
    }
  }
}
</script>
<style>
.Mon {
  margin-top: 100px;
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: space-evenly;
}
.card {
  width: 200px;
  height: 200px;
  margin-top: 40px;
  border: 3px solid black;
  box-shadow: 1px 1px 1px;
}
.addTeam {
  width: 50px;
  height: 50px;
}
</style>

<template>
  <body>
    <h1>21</h1>
    <div class="Mon">
      <div class="card" v-for="pokemon in pokemons">
        <p>{{ pokemon.name }}</p>

        <button class="addTeam">
          <p>ADD TO TEAM</p>
          {{ pokemon.name }} <img :src="pokemon.url" />
        </button>
      </div>
    </div>
  </body>
</template>
<!-- data() { return { items: [{ message: 'Foo' },{ message: 'Bar' }] } } template
<li v-for="item in items">
  {{ item.message }}
</li> -->
