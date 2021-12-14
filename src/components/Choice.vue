<template>

    <div id="faculties_symbols">
        <img :src="require('@/assets/'+ card.img)" alt="">
        <p>{{card.nome}}</p>
    </div>
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

#faculties_symbols{
    border: 1px solid rgb(231, 229, 229);
    padding: 20px; 
}

#faculties_symbols img{
    display: flex;
    width: 50%;
    margin: 0 auto;
    padding:20px;
}

#faculties_symbols p{
    text-align: center;
    color: #e56768;
    font-weight: 800;
    color: #80828c;
}

</style>