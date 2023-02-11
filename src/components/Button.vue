<template>
    <button @click="onClick()">
      {{ text }}
    </button>
  </template>
  
  <script lang="ts">
  import { defineComponent } from "vue";
  export default defineComponent({
    name: "BtnComp",
    props: {
      text: String,
    },
    methods: {
      onClick() {
        this.$emit("btn-click");
      },
    },
  });
  </script>
  
  <style scoped lang="scss">
  button {
    padding: 0.7rem;
    color: #fff;
    font-size: 1.2rem;
    border: none;
    background-color: #050505;
    border-bottom: 4px solid #494246;
    border-radius: 30%;
    &:hover {
      cursor: pointer;
      background-color: #494246;
    }
  }
  </style>