<template>
  <div class="scrollClass">
      <b-card-group columns :key="film.id" v-for="film in films" >
        <FilmCard :film="film"/>
      </b-card-group>
      
  </div>
</template>

<script>

import FilmCard from './FilmCard.vue'

export default {
    components: {
        FilmCard
    },

    data: function() {
            return { 
                films: [
                    {id: 1, name: 'Rocky', rating: 3, image: require('../assets/rocky.jpeg'),  summary: 'bref summary', detail: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse malesuada hendrerit mauris, ut sollicitudin dui placerat quis. Curabitur sollicitudin non sapien nec iaculis. Suspendisse bibendum magna elit. Duis id luctus erat. Mauris ultricies sodales fermentum. Nullam non semper nulla, sit amet finibus mi. Cras sed dui vel ante porttitor sodales sit amet laoreet urna.'},
                    {id: 2, name: 'DeadPool', rating: 5, image: require('../assets/deadpool.jpeg')},
                    {id: 3, name: 'La La Land', rating: 0, image: require('../assets/lalaland.jpeg')}
                ]            
            }
    }
    
}

</script>

<style>
.scrollClass {
    height: auto;
  overflow-y: scroll;
}
</style>