<script>
export default {
  data() {
    return {
      pokemons: [
        {
          name: 'Charizard',
          url: 'https://st.depositphotos.com/2935381/4237/i/950/depositphotos_42373695-stock-photo-grey-paper-texture-or-background.jpg'
        },
        { name: 'Charmander' },
        { name: 'Blastoise' }
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
