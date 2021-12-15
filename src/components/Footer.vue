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

    <!-- third section -->
    <section id="third_section">
       <!-- left -->
      <div id="left_part">
        <img :src="require('@/assets/theme_eduprime_logo.png')" alt="Clock">
        <p>Eduprime is the most versatile Wordpress theme for <br>
           educational pourpouse, showcasing universities <br>
           courses,secondary school etc. 
        </p>
        <div id="social">
          <i class="fab fa-facebook-f fa-1x"></i>
          <i class="fab fa-twitter fa-1x"></i>
          <i class="fab fa-instagram fa-1x"></i>
        </div>
      </div>
          
      <div id="center_part">
        <!-- center -->
        <div id="footer_list">
          <h5>Get EduPrime</h5>
              <Services 
              v-for="purchase in servicesList"
              :key="purchase.id"
              :sevices_offered="purchase"
              />
        </div>    
        <div>
          <h5>Networking</h5>
            <Network 
              v-for="theme in networkList"
              :key="theme.id"
              :benefits="theme"
            />
        </div>
      </div>
    </section>
</template>

<script>

import Brands from '@/components/Brands.vue'
import Services from '@/components/Services.vue'
import Network from '@/components/Network.vue'

export default {
   name:'Footer',
   components:{
   Brands,
   Services,
   Network
  },
  data(){
    return{
      shopList:[
        {
          item:'partner-1.png',
          id:1
        },
        {
          item:'partner-2.png',
          id:2
        },
        {
          item:'partner-3.png',
          id:3
        },
        {
          item:'partner-4.png',
          id:4
        },
        {
          item:'partner-5.png',
          id:5
        },
        {
          item:'partner-6.png',
          id:6
        },
        {
          item:'partner-7.png',
          id:7
        },
        {
          item:'partner-8.png',
          id:8
        }
      ],

      servicesList:[
        {
          action:'Request a website',
          id:1
        },
        {
          action:'Browse Themes',
          id:2
        },
        {
          action:'Payment options',
          id:3
        },
        {
          action:'Support System',
          id:4
        },
        {
          action:'Checkout',
          id:5
        },
        {
          action:'Purchase Theme',
          id:6
        }
      ],

      networkList:[
        {
          step:'Purchase Theme',
          id:1
        },
        {
          step:'Our Benefits',
          id:2
        },
        {
          step:'Our team',
          id:3
        },
        {
          step:'Our Services',
          id:4
        },
        {
          step:'Other Products',
          id:5
        },
        {
          step:'My Account',
          id:6
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

/* third section */

  /* left */
#third_section{
  background-color: #e56768;
  display: flex;
  justify-content: space-around;
}

#left_part{
  padding: 50px;
}

#left_part > img{
  width:300px;
}

#left_part > p{
  color: white;
  padding: 30px 0;
  line-height:20px;
}

#social i{
  border: 1px solid yellow;
  border-radius: 50px;
  padding:5px 6px;
  margin:5px;
  
}

  /* center */

  #center_part{
    display: flex;
    padding: 80px 0px;
    line-height:30px;
    color:white;
  }

  #footer_list{
    padding: 0 40px;

  }


</style>