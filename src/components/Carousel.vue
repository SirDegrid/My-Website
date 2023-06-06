<template>
    <div id="example">
      <carousel :perPageCustom="[[480, 1], [768, 1]]">
        <slide v-for="item in items" :key="item.id">
            <SlideDisplay :title="item.title" :description="item.description" :link="item.link" />
        </slide>
      </carousel>
    </div>
</template>

  
  <script>
  import { Carousel, Slide } from 'vue-carousel';
  import SlideDisplay from './SlideDisplay.vue';
  
  export default {
    components: {
      Carousel,
      Slide,
      SlideDisplay,
    },
    data() {
    return {
      items: [
        {
          id: 1,
          title: 'Beef Butcher',
          description: 'Ruby on Rails application demonstrating the creation of databases, full CRUD features and associations.',
          link: 'http://placekitten.com/g/200/300'
        },
        {
          id: 2,
          title: 'BarPretender',
          description: 'Ruby on Rails back end and React front end. Helping users find cocktail recipes based on ingredients at hand.',
          link: 'http://placekitten.com/g/200/300'
        },
        {
          id: 3,
          title: 'Harvestable',
          description: 'Unusre. Hoping to have this done by the end of next week. Book servies.',
          link: 'http://placekitten.com/g/200/300'
        },
      ],
    };
  },
};
</script>

<style scoped>
.VueCarousel-slide {
  position: relative;
  background-color: beige;
  color: black;
  font-family: Arial;
  font-size: 24px;
  text-align: center;
  min-height: 350px;
  border: 1px solid black;
  box-sizing: border-box;
}

</style>
  
  <style scoped>
  .VueCarousel-slide {
    position: relative;
    background-color: beige;
    color: black;
    font-family: Arial;
    font-size: 24px;
    text-align: center;
    min-height: 350px;
    border: 1px solid black;
    box-sizing: border-box;
  }
  
  /* Add your custom styles for SlideDisplay here */
  </style>
  