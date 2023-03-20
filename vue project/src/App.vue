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

<template>
  <header>
    <button>1231</button>
    <li v-for="pokemon in pokemons" in>{{ pokemon.name }} <img :src="pokemon.url" /></li>
  </header>
</template>

<!-- data() { return { items: [{ message: 'Foo' }, { message: 'Bar' }] } } template
<li v-for="item in items">
  {{ item.message }}
</li> -->
