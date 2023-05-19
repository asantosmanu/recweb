<script setup>
import { livros } from '@/_data/livros.js'
  </script>

<template>
  <h1> livraria (de novo)</h1>
  <div class="listagem-livros">
    <div class="card-livro" v-for="livro in livros" :key="livro.id">
      <img src="livro.img" alt="capa do livro" class="capa-livro" />
      <p class="titulo-livros">{{ livros.title }}</p>
      <p class="titulo-autor">{{ livros.author }}</p>
      <p class="titulo-preco">{{ livros.price }}</p>
     <!-- {{ livro}} -->
    </div>
  </div>

</template>

<style scoped>
h1{
  color: black;
  
}
.listagem-livros{
  display: flex;
  flex-wrap: wrap;

}
.capa-livro{
  width: 250px;
  padding: 10px;
  background-color: beige;
  border-radius: 5px;
}
</style>
