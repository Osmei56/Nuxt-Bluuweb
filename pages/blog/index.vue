<template>
  <div class="container mt-5">
    <div class="row">
      <div class="col-md-3"
      v-for="(articulo, index) in articulos" :key="index">
        <h2><nuxt-link :to="`/blog/${ articulo.id }`">{{ articulo.titulo }}</nuxt-link></h2>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      articulos: [
        {id: 1, titulo: 'Titulo #1'},
        {id: 2, titulo: 'Titulo #2'},
        {id: 3, titulo: 'Titulo #3'},
        {id: 4, titulo: 'Titulo #4'},
        {id: 5, titulo: 'Titulo #5'}
      ]
    }
  }
}
</script>