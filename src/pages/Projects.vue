<template>
    <Layout>
      <h1>Projects</h1>
      <CarouselComponent/>
    </Layout>
  </template>
  
  <script>
import CarouselComponent from '@/components/Carousel.vue'
  
  export default {
    metaInfo: {
      title: 'Projects'
    },
    components: {
      CarouselComponent
    }
  }
  </script>
  