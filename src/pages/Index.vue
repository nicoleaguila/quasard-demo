<template>
  <div class="row q-ma-md q-pa-ml q-pl-xl items-center q-gutter-md">
    <q-card class="my-card col-3 col-ls-auto col-xs-auto" v-for="personaje in personajes" :key="personaje.id">
      <img :src="personaje.imagen">

      <q-card-section>
        <div class="text-h6 q-pa-md q-gutter-lg">{{ personaje.nombre }}</div>
      </q-card-section>
    </q-card>

  </div>
</template>

<script>
export default {
  name: 'PageIndex',
  data () {
    return {
      personajes: [
        {
          id: 1,
          nombre: 'Morty',
          imagen: 'https://rickandmortyapi.com/api/character/avatar/2.jpeg'
        },
        {
          id: 2,
          nombre: 'Rick',
          imagen: 'https://rickandmortyapi.com/api/character/avatar/1.jpeg'
        },
        {
          id: 3,
          nombre: 'Summer',
          imagen: 'https://rickandmortyapi.com/api/character/avatar/3.jpeg'
        },
        {
          id: 4,
          nombre: 'Beth',
          imagen: 'https://rickandmortyapi.com/api/character/avatar/4.jpeg'
        },
        {
          id: 5,
          nombre: 'Jerry',
          imagen: 'https://rickandmortyapi.com/api/character/avatar/5.jpeg'
        }
      ]
    }
  }

}
</script>
