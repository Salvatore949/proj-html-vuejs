<template>
  <div id="logosBrand">
      <img :src="require('@/assets/'+ logos.item)" alt="">
  </div>
</template>

<script>

export default {
   name:"Brands",
    props: {
    logos:Object
  }
}
</script>

<style>

#logosBrand > img{
    width: 50px;
    height:40px;
    padding: 0 20px;
}

</style>