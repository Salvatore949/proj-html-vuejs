<template>

  <!-- first section -->
  <section>
    <div id="red_bar">
      <p>SubScribe Now to our Newsletter</p>
      <div>
        <input id="insert" type="text" placeholder="Email address..">
        <button><i class="fas fa-paper-plane"></i></button>
      </div>
    </div>
  </section>

  <!-- second section -->
  <section>
    <div id="logos_paragraph">
      <h2>Partners</h2>
      <p>Levarage agile frameworks to provide a robust synopsis for high level <br>
        overviews. Iterative approaches to comparate strategy
      </p>
    </div>
    <div id="logos">
      <brands 
        v-for="made in shopList"
        :key="made.id"
        :logos="made"/>
    </div>
  </section>
   
</template>

<script>

import Brands from '@/components/Brands.vue'

export default {
   name:'Footer',
   components:{
   Brands
  },
  data(){
    return{
      shopList:[
        {
          item:'partner-1.png',
          id:"1"
        },
        {
          item:'partner-2.png',
          id:"2"
        },
        {
          item:'partner-3.png',
          id:"3"
        },
        {
          item:'partner-4.png',
          id:"4"
        },
        {
          item:'partner-5.png',
          id:"5"
        },
        {
          item:'partner-6.png',
          id:"6"
        },
        {
          item:'partner-7.png',
          id:"7"
        },
        {
          item:'partner-8.png',
          id:"8"
        }
      ]
    }
  }
}
</script>

<style>
/* first section */

#red_bar{
    background-color:#e56768;
    display: flex;
    justify-content: space-around;
    color: white;
    font-size: 30px;
    padding: 30px 0;

}

#insert{
    padding:8px 50px;
    border-radius: 30px;
    border:none;
}

#red_bar button{
    padding:8px 0px;
    color: white;
    background-color:#e9d758;
    border:none;
    border-radius:50px;
    width: 33px;
    margin-left:-25px
}

#red_bar p{
    margin-top: 5px;
}

/* second section */
#logos{
  display: flex;
  justify-content: center;
  padding-bottom:50px;
}

#logos_paragraph{
  text-align: center;
}

#logos_paragraph p{
  padding: 20px;
  color: #434655;
}

#logos_paragraph h2{
  padding: 60px 0 10px ;
  font-size:40px;
}
</style>