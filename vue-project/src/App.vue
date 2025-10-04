<script setup>
import { ref } from 'vue'
import Footer from './Footer.vue';
import Navbar from './navbar.vue';
import Lista from './Lista.vue';

const nombre = ref('Polux')
const libros = ref(4)
function nombrelibros () {
  return (`${nombre.value} es un personaje que aparece en ${libros.value} libros`)
}

</script>

<template>

  <Navbar />

  <h1>Vue Project 1</h1>
  <p>{{ nombrelibros() }}</p>

  <h3>Resultado de una operacion</h3>  
  <p>3 + 3 = {{  3 + 3 }}</p>

  <Lista />

  <Footer />
  
</template>

<style scoped></style>
