<template>
  <div id="post_card">
      <div id="single_card">
          <img :src="require('@/assets/'+ opportunity.img)" alt="">
          <h5>{{opportunity.subtile}}</h5>
          <p>Teacher:<strong>{{opportunity.teacher}}</strong></p>
          <p>Price:strong <strong>{{opportunity.money}}</strong></p>
      </div>
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

#post_card{
  display: flex;
  flex-direction:column ;
}

#single_card{
  width: 65%;
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

#post_card > button{
  width: 120px;
  margin-left:60px;
  margin-top: -25px;
  background-color: #e56768;
  border: none;
  border-radius:40px;
  padding: 10px;
  color: white;
  font-weight: 800;

}

</style>