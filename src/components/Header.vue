<template>
    <header>
      <h1>Pokédex - Marcos</h1>
    </header>
  </template>
  
  <script lang="ts">
  export default {
    name: "PokeHeader",
    props: {
      title: String,
      showAddTask: Boolean,
    },
  };
  </script>
  
  <style scoped lang="scss">
  header {
    padding: 0.5rem 1;
    background-color: #5f073d;
    h1 {
      color: #f5f2f2;
      border-bottom: 2px solid #f8f8f8;
    }
  }
  </style>