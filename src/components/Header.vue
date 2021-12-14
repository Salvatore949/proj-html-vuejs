<template>
<!-- header bar -->
  <header>
    <nav>
      <!-- right part -->
      <div id="logo">
        <img :src="require('@/assets/theme_eduprime_logo.png')" alt="Logo">
      </div>
      <!-- left part -->
      <div id="buttons">
        <Options 
        v-for="selected in optionsList"
        :key="selected.id"
        :details="selected"
        />
        <button id="courses"> VIEW COURSES</button>
      </div>
    </nav>
  </header>
</template>

<script>

import Options from '@/components/Options.vue'

export default {
  name:'Header',
  components:{
    Options
  },
   data(){
    return {
      optionsList: [
        {
          name:"Home",
          img:"fas fa-sort-down",
          id:1
        },

        {
          name:"Courses",
          img:"fas fa-sort-down",
          id:2
        },

        {
          name:"About Us",
          img:"fas fa-sort-down",
          id:3
        },

        {
          name:"News",
          img:"fas fa-sort-down",
          id:4
        },

        {
          name:"Pages",
          img:"fas fa-sort-down",
          id:5
        },

        {
          name:"Contact",
          img:"fas fa-sort-down",
          id:6
        },

        {
          name:"Purchase",
          img:"fas fa-sort-down",
          id:7
        }
      ]
    }
  }
}
</script>

<style>

  *{
    margin: 0;
    padding: 0;
  }

  #logo img{
    width: 40%;
  }

  nav{
    background-color: #d4686d;
    display: flex;
    justify-content: space-between;
    padding:20px;
  
  }

  #courses{
     background: #e9d758;
     border:0;
     border-radius: 50px;
     padding:15px;
     color:white;
  }

  #buttons{
    display: flex;
    color:white;
  }



</style>