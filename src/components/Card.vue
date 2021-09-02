<template>
  <div>
    <v-container class="grey lighten-5">
      <v-row row--dense>
        <v-col
          v-for="(personaje, index) in personajes"
          :key="index"
          cols="12"
          sm="4"
        >
          <v-card class="m-3" outlined tile>
            <v-card class="mx-auto">
              <v-img :src="personaje.imagen" ></v-img>

              <v-card-title> {{ personaje.nombre }} </v-card-title>
            </v-card>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>
<script>
export default {
  data() {
    return {
      personajes: [
        {
          id: 1,
          nombre: "Morty",
          imagen: "https://rickandmortyapi.com/api/character/avatar/2.jpeg",
        },
        {
          id: 2,
          nombre: "Rick",
          imagen: "https://rickandmortyapi.com/api/character/avatar/1.jpeg",
        },
        {
          id: 3,
          nombre: "Summer",
          imagen: "https://rickandmortyapi.com/api/character/avatar/3.jpeg",
        },
        {
          id: 4,
          nombre: "Beth",
          imagen: "https://rickandmortyapi.com/api/character/avatar/4.jpeg",
        },
        {
          id: 5,
          nombre: "Jerry",
          imagen: "https://rickandmortyapi.com/api/character/avatar/5.jpeg",
        },
         {
          id: 6,
          nombre: "Abadango",
          imagen: "https://rickandmortyapi.com/api/character/avatar/6.jpeg",
        },
      ],
    };
  },
};
</script>

<style>
</style>