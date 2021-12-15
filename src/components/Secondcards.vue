<template>
    <div id="single_card">
        <img :src="require('@/assets/'+ opportunity.img)" alt="">
        <h5>{{opportunity.subtile}}</h5>
        <p>Teacher:<strong>{{opportunity.teacher}}</strong></p>
        <p>Price:strong <strong>{{opportunity.money}}</strong></p>
        <button>View Course</button>
    </div>
</template>

<script>
export default {
  name:"Secondcards",
    props: {
    opportunity: Object
  }
}
</script>

<style>

#single_card{
  width: 10%;
  text-align: center;
  margin:10px;
  padding:30px;
  line-height: 25px;
  box-shadow: 2px 12px 10px #ebe5e5;

}

#single_card img{
  width:80px;
}

#single_card > p{
  color:#6c6e7b;
}

</style>