<template>
    <img :src="require('@/assets/'+ card.img)" alt="">
    <p>{{card.nome}}</p>
</template>

<script>
export default {
 name:'Choice',
   props: {
    card:Object
  }
}
</script>

<style>



</style>