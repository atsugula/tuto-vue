<script setup>
  const name = 'Vue 3';
  const styleAzul = 'color: blue';
  const styleAmarillo = 'color: yellow';
  const arrayColores = ['red','yellow','orange','peru'];
  const condicional = true;
</script>

<template>
  <h1>Hola mundo, {{ name }}</h1>
  <h2 v-bind:style="styleAzul">color azul</h2>
  <h2 :style="styleAmarillo">color amarillo</h2>
  <h2 :style="`color: ${arrayColores[3]}`">color Perú</h2>
  <h3>{{ condicional ? 'Es verdad' : 'Es falso' }}</h3>
</template>

<style>
  h1{
    color:red
  }
</style>