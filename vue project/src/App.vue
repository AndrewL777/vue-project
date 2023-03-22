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
.card {
  width: 150px;
  height: 150px;
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
  <header>
    <h1>r[fie eur tyeam]</h1>
    <div class="card" v-for="pokemon in pokemons">
      <button class="addTeam">{{ pokemon.name }} <img :src="pokemon.url" /></button>
    </div>
  </header>
</template>

<!-- data() { return { items: [{ message: 'Foo' },{ message: 'Bar' }] } } template
<li v-for="item in items">
  {{ item.message }}
</li> -->
