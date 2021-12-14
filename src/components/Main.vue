<template>
    <main>

        <!-- first section -->
        <section id="first-section">
            <!-- left part -->
            <div id="first-section_id">
                <img id ="books" :src="require('@/assets/Books-icon.png')" alt="">
                <h2>Thousand of courses <br>
                    for any type of student</h2>
                <p>At EduPrime it doesn't matter what the domain you wish to pursue a career in. Here you <br> 
                can find a person that satisfies your needs within a click away and applies for a course <br>
                in a matter of minutes. EduPrime is ranked as the most university in the <br>
                world, thanks to the number of courses it provides</p>
                <button>Browse through courses</button>
            </div>
            <!-- right part -->
            <img id="bachelor" :src= "require('@/assets/Graduation-Illustration.png')" alt="">
            <!-- <img id="point" :src= "require('@/assets/home-background.png')" alt=""> -->
        </section>

        <!-- second section -->
        <section>
            <!-- centered -->
            <div id="faculties_available">
                <h2>Faculties available at EduPrime</h2>
                <p>A single University with a load of courses, tailored <br>
                to satisfy any student's need</p>
            </div>
            <div id="faculties_symbols">
              <Choice 
               v-for="schools in facultiesChoice"
               :key="schools.id"
               :card="schools"
              />
            </div>
        </section>


        <!-- third section -->
        <section id="gavel">
            <!-- left div -->
            <img :src="require('@/assets/Gavel-Illustration-e1556884768193.png')" alt="">
            <!-- right div -->
            <div id="gavel_text">
                <h2>Law Faculty</h2>
                <p>Learning from World leading academics and practitioners will not only receive <br>
                    and outstanding grounding in the Theory of love like you will be able to understand <br>
                    how those principles are applied in practise is through a range of student-led <br>
                    activities and competitions</p>
                <button>Read More</button>
            </div>
        </section>

    </main>  
</template>

<script>
import Choice from '@/components/Choice.vue'
export default {
  name:'Main',
  components:{
   Choice
  },
  data(){
      return{
          facultiesChoice: [
              {
                  img:"Gavel-v2.png",
                  nome:"Law Faculty",
                  id:1
              },
              {
                  img:"Coins-tabs-v2.png",
                  nome:"Economy",
                  id:2
              },

              {
                  img:"Medicine.png",
                  nome:"Medicine",
                  id:3
              },

              {
                  img:"Computer-tabs-v2.png",
                  nome:"Computer Science",
                  id:4
              },

              {
                  img:"Palette-tabs-v2.png",
                  nome:"Graphic Designe",
                  id:5
              }
          ]
      }
  }
}
</script>

<style>
 
/*first section*/

#first-section{
    display: flex;
    width: 70%;
    margin:30px auto;
}

#books{
    width: 50px;
    margin-bottom: 20px;
}

#first-section h2{
    font-size: 35px;
    margin-bottom: 40px;
}

#first-section_id > p{
    line-height: 25px;
}

#first-section_id > button{
    padding:15px 50px;
    background-color: #e9d758;
    border:none;
    color:white;
    border-radius:50px;
    margin-top: 40px;
    font-weight: 800;
}

#first-section > #bachelor{
    width:370px;
    height: 300px;
    margin-left: 100px;
    display: flex;
    margin-top:70px;

}


/*second section*/

#faculties_available{
    text-align: center;
    padding-top: 150px;
}

#faculties_available > h2{
    padding-bottom:30px;
    font-size:35px;
}

#faculties_available > p{
    font-size:17px;
    line-height: 22px;
}

#faculties_symbols{
    border: 1px solid grey; 
    display: flex;
    justify-content: center;  
    margin-top: 30px;
}

#faculties_symbols > img{
    width:10%;
    padding:40px;
    border: 1px solid rgb(172, 167, 167);
}

/*third section*/

#gavel{
    display: flex;
    width: 70%;
    margin: 0 auto;
    padding: 100px;
}

#gavel img{
    padding-right: 60px;
}

#gavel_text{
    display:flex;
    flex-direction: column;
    justify-content: center;
    line-height:30px;
}

#gavel_text button{
    width: 30%;
    padding: 10px 6px;
    border-radius: 50px;
    border:none;
    background-color: #e56768;
    color: white;
}

#gavel_text p{
    padding:30px 0;
}


</style>