<template>
  <div class="home">
    <CategoriesGrid/>
  </div>
</template>

<script>
  import Stepper from '@/components/stepper.vue'
  import CategoriesGrid from '@/components/categoriesGrid.vue'
  import CardCategory from '@/components/cardCategory.vue'
  
  export default {
    name: 'home',
    components: {
      Stepper,
      CategoriesGrid,
      CardCategory
    }
  }
</script>


