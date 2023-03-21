<script>
export default {
  data() {
    return {
      pokemons: [
        {
          name: '',
          url: ''
        },
        { name: '', url: '' },
        { name: '', url: '' },
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
  width: 35.4rem;
  height: 23.4rem;

  border: 3px solid black;
  box-shadow: 5px 5px 15px;
}
</style>

<template>
  <header>
    <h1>Pick</h1>
    <div class="card" v-for="pokemon in pokemons">
      {{ pokemon.name }} <img :src="pokemon.url" />
    </div>
  </header>
</template>

<!-- data() { return { items: [{ message: 'Foo' },{ message: 'Bar' }] } } template
<li v-for="item in items">
  {{ item.message }}
</li> -->
