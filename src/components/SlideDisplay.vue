<template>
    <div class="slide-display">
      <h2>{{ title }}</h2>
      <p>{{ description }}</p>
      <a :href="link" target="_blank">Click here for more information</a>
    </div>
  </template>
  
  <script>
  export default {
    props: {
      title: {
        type: String,
        required: true,
      },
      description: {
        type: String,
        required: true,
      },
      link: {
        type: String,
        required: false,
      },
    },
  };
  </script>
  
  <style scoped>
  .slide-display {
  }
  </style>
  