<template>
  <div>
    <h1>{{ titulo }}</h1>
    <ul>
      <li v-for="foto of fotos">
        <img :src="foto.url" :alt="foto.titulo">
      </li>
    </ul>
  </div>
</template>

<script>
export default {

  data() {
    return {
      titulo: 'Alurapic',
      fotos: [
        {
          url: 'https://image.cnbcfm.com/api/v1/image/105992231-1561667465295gettyimages-521697453.jpeg?v=1561667497',
          titulo: 'cachorro'
        },
        {
          url: 'https://image.cnbcfm.com/api/v1/image/105992231-1561667465295gettyimages-521697453.jpeg?v=1561667497',
          titulo: 'cachorrão'
        }
      ]
    }
  }
}
</script>

<style>

</style>
