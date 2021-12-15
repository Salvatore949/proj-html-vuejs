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
            </div >
            <div id="whole_div">
                <div id="whole_faculties">
                    <Choice 
                    v-for="schools in facultiesChoice"
                    :key="schools.id"
                    :card="schools"
                    />
                </div>
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

        <!-- fourth section -->
        <section id="red_part">
            <!-- first title -->
            <div id="heading">
                <img :src="require('@/assets/Clock-and-Bell.png')" alt="">
                <h2>University Year</h2>
            </div>
            <div id="line">

                <div id="red_part_up">
                    <p>
                        <strong>Demo classes</strong><br>
                            In in the first week students try to accommodate with the <br>
                            teaching style and choose their optional courses. <br>
                    </p>
                    <p>
                        <strong>Graduation</strong><br>
                            On the day of graduation all students gather for this <br>
                            ceremony and then network and party among others. <br>
                    </p>
                </div>
                 <img id="step_line" :src="require('@/assets/Timeline-Item.png')" alt="">

                <div id="red_part_down">
                    <p>
                        <strong>Orientation</strong><br>
                            First day of the university here oll students gather for<br>
                            the opening ceremony and then network with others.<br>
                    </p>
                    <p>
                          <strong>Evaluation</strong><br>
                            At the end of a semester students take a general<br>
                            evaluation test for every subject their learning.<br>
                    </p>
                </div>
            </div>
            <!-- second title -->
            <div id="lower_part">
                <div id="lower_header">
                    <img :src="require('@/assets/upcoming-events-calendar-icon.png')" alt="">
                    <h2>Upcoming Events</h2>
                </div>
                <div id="coaching_session">
                    <!-- left event -->
                    <div id="event">
                        <img src="" alt="">
                        <h4>Coaching session</h4>
                        <p> 20 May 21.30 PM</p>
                        <p>Lorem ipsum dolor sit amet consectetur <br>
                        adipisicing elit, sed do eiusmod tempor[...]</p>
                        <button> + find more </button>
                    </div>
                    <!-- center event -->
                    <div id="event">
                        <h4>Coaching session</h4>
                        <p> 24 Mar 18.00 PM</p>
                        <p>Lorem ipsum dolor sit amet consectetur <br>
                        adipisicing elit, sed do eiusmod tempor[...]</p>
                        <button> + find more </button>
                    </div>
                <!-- right event -->
                    <div id="event">
                        <h4>Coaching session</h4>
                        <p> 12 Feb 13.30 PM</p>
                        <p>Lorem ipsum dolor sit amet consectetur <br>
                        adipisicing elit, sed do eiusmod tempor[...]</p>
                        <button> + find more </button>
                    </div>
                </div>
                <button>View All Events</button>
            </div>
        </section>


        <!-- fifth section -->
        <section>
            <h2 id="fifth_head">Latest Courses</h2>
            <div id="cards">
               <Secondcards
               v-for="skils in cardList"
               :key="skils.id"
               :opportunity="skils"
                />
            </div>
        </section>

        <!-- sixth section -->
        <section id="sixth_section">
            <div id="sixth_left">
                <img :src="require('@/assets/Exam-icon.png')" alt="">
                <h2>The most efficient <br>
                    examination method
                </h2>
                <p>Edu prime is gathered teachers from Around The Globe to <br>
                   brainstorm in Order to facilitate di evaluation of Our students <br>
                   Every teacher from our University has an influence on how <br>
                   students are evaluated and is subject
                </p>
                <button>Discover the method</button>
            </div>
            <img :src="require('@/assets/Exam-Illustration.png')" alt="">
        </section>


        <!-- seventh section -->
        <section id="seventh_section">
            <img :src="require('@/assets/Girl-Illustration.png')" alt="">
            <div id="seventh_right">
                <img :src="require('@/assets/Exam-icon-1.png')" alt="">
                <h2>Variable fees for<br>
                    international students</h2>
                <p>Edu prime is gathered teachers from Around The Globe to <br>
                   brainstorm in Order to facilitate di evaluation of Our students <br>
                   Every teacher from our University has an influence on how <br>
                   students are evaluated and is subject
                </p>                
                <button>Discover the method</button>
            </div>

        </section>
         
        <!-- eighth section -->

        <section>
            <div id="red_bar">
             <p>SubScribe Now to our Newsletter</p>
             <input id="insert" type="text" placeholder="Email address..">
             <button></button>
            </div>
        </section>


    </main>  
</template>

<script>
import Choice from '@/components/Choice.vue'
import Secondcards from '@/components/Secondcards.vue'
export default {
  name:'Main',
  components:{
   Choice,
   Secondcards
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
                  img:"Medicine-tabs-v2.png",
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
          ],

            cardList: [
                {
                    img:'Decisions-icon.png',
                    subtile:'Make Better Decision',
                    teacher:'James Colins',
                    money:'$21.00',
                    id:1
                },

                {
                    img:'Speaker-icon.png',
                    subtile:'How to be a speaker',
                    teacher:'James Colins',
                    money:'free',
                    id:2
                },

                {
                    img:'Network-icon.png',
                    subtile:'Network Introductions',
                    teacher:'James Colins',
                    money:'free',
                    id:3
                },

                {
                    img:'Brand-icon.png',
                    subtile:'Brand Management',
                    teacher:'James Colins',
                    money:'free',
                    id:4
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
    /* background:url('../assets/theme_slider1_bg-1.jpg'); */
}

#books{
    width: 50px;
    margin-bottom: 20px;
}

#first-section h2{
    font-size: 35px;
    margin-bottom: 40px;
    color: #3d404f;

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
    padding-top: 70px;
}

#faculties_available > h2{
    padding-bottom:30px;
    font-size:35px;
    color:#3d404f;
}

#faculties_available > p{
    font-size:17px;
    line-height: 22px;
    color: #80828c;
}

#whole_div{
    border-top: 1px solid rgb(228, 223, 223);
    border-bottom: 1px solid rgb(233, 231, 231);
    margin: 40px 0 20px;
    box-shadow: 2px 12px 30px #f5f0f0;
}

#whole_faculties{
    display: flex;
    width: 80%;
    margin: 0 auto;
}
/*third section*/

#gavel{
    display: flex;
    width: 70%;
    margin-left: 200px;
    padding: 50px 100px;
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

#gavel_text h2{
    color:#434959;
}

#gavel_text p{
    padding:30px 0;
    color: #80828c;
}

/*fourth section*/
#red_part{
    background-color: #e56768;
}
#heading{
    text-align: center;
}

#heading h2{
    font-size: 30px;
    padding-top:30px;
    color: white;
}

#heading img{
    width:80px;
    padding-top:60px;
}

#line{
    width: 80%;
    margin:0 auto;
}

#step_line {
    margin: 30px;
}

#red_part_up{
    display: flex;
    color: white;
    margin-left:180px;
}

#red_part_up p{
    text-align: center;
    padding: 80px 0px 0;
    margin-left: 150px;
}

#red_part_down{
    display: flex;
    color: white;
}

#red_part_down p{
    text-align: center;
    padding: 0 95px;
}

/* Lower part */

#lower_header{
    text-align: center; 
    padding:40px 40px;
}

#lower_header > h2{
    padding-top:10px;
    color: white;
    font-size: 40px;
}

#lower_header > img{
    width: 50px;
}

#lower_part > button {
    padding:13px;
    border-radius:50px;
    background-color:#e9d758;
    border:none;
    color: white;
    font-weight: 800;
    width: 180px;
}

#coaching_session{
    display: flex;
    margin: 0 auto;
    text-align: center;
    padding: 30px;
    width: 70%;
}

#event{
    padding: 20px 50px;
    background-color:#ffffff;
    border-radius: 10px;
    margin: 15px;
}

#event > button {
    background-color:#e56768 ;
    border-radius: 30px;
    padding: 10px;
    border:none;
    color: white;

}

/* fifth section */

#fifth_head{
    padding:40px;
    margin-left: 262px;
}

#cards{
    display: flex;
    justify-content: center;
}

/* sixth section */

#sixth_section{
    display: flex;
    justify-content: center;
    padding: 20px 0;
}

#sixth_left > button {
    width: 180px;
    padding:10px 0;
    background-color: #e56768;
    border:none;
    border-radius: 50px;
}

#sixth_section p{
    padding:30px 50px 30px 0px;
}

#sixth_section img{
    width: 30%;
    padding:20px 0;
}

#sixth_left{
    display: flex;
    flex-direction:column;
    justify-content: center;
}

#sixth_left img{
    width: 40px;
}

/* seventh section */

#seventh_section{
    display: flex;
    justify-content: center;
    padding: 100px 0;
}

#seventh_right > button {
    width: 180px;
    padding:10px 0;
    background-color: #e56768;
    border:none;
    border-radius: 50px;
}

#seventh_section p{
    padding:30px 0;
}

#seventh_section img{
    width: 30%;
}

#seventh_right img{
    width: 40px;
    padding:20px 0;
}

#seventh_right{
    display: flex;
    flex-direction:column;
    justify-content: center;
    padding-left:70px ;
}

/* eighth section */

#red_bar{
    background-color:#e56768;
}

#red_bar{
    color: white;
    font-size: 30px;
}

#insert{
    padding:8px 50px;
    border-radius: 30px;
    border:none;
}
</style>