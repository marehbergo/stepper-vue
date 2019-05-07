<template>
  <v-layout row wrap>
    <v-flex xs12 text--xs--center>
      <v-container 
        v-bind:style="{backgroundColor: '#EEEEEE'}"
        pa-3 ma-0
        grid-list-lg
        text--xs--center
      >
        <v-layout row wrap>
          <v-flex v-for="i in 5" :key="`6${i}`" xs6>
            <CardCategory/>
          </v-flex>
        </v-layout>
      </v-container>
    </v-flex>
  </v-layout>
</template>

<script>
  import CardCategory from '@/components/cardCategory.vue'
  
  export default {
    name: 'CategoriesGrid',
    components: {
      CardCategory
    },
    data () {
      return {
        //
      }
    }
  }
</script>
