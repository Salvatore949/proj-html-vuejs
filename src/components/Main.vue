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
            <h2>Upcoming Events</h2>
            <div id="coaching_session">
                <!-- left event -->
                <div id="left_event">
                    <h4>Coaching session</h4>
                    <p> 20 May 21.30 PM</p>
                    <p>Lorem ipsum dolor sit amet consectetur <br>
                       adipisicing elit, sed do eiusmod tempor[...]</p>
                    <button> + find more </button>
                </div>
                <!-- center event -->
                <div id="center_event">
                    <h4>Coaching session</h4>
                    <p> 24 Mar 18.00 PM</p>
                    <p>Lorem ipsum dolor sit amet consectetur <br>
                       adipisicing elit, sed do eiusmod tempor[...]</p>
                    <button> + find more </button>
                </div>
               <!-- right event -->
                <div id="right_event">
                    <h4>Coaching session</h4>
                    <p> 12 Feb 13.30 PM</p>
                    <p>Lorem ipsum dolor sit amet consectetur <br>
                       adipisicing elit, sed do eiusmod tempor[...]</p>
                    <button> + find more </button>
                </div>
            </div>
        </section>


        <!-- fifth section -->
        <section>
            <h2>Latest Courses</h2>
            <div id="cards">
            <!-- first card -->            
                <div id="single_card">
                    <img src="" alt="">
                    <h5>Make Better Decisions</h5>
                    <p>Teacher:<strong>James Colins</strong></p>
                    <p>Price:strong <strong>$21.00</strong></p>
                    <button>View Course</button>
                </div>
            <!-- second card -->
                <div id="single_card">
                    <img src="" alt="">
                    <h5>Make Better Decisions</h5>
                    <p>Teacher:<strong>James Colins</strong></p>
                    <p>Price:strong <strong>$21.00</strong></p>
                    <button>View Course</button>
                </div>
            <!-- third card -->
                <div id="single_card">
                    <img src="" alt="">
                    <h5>Make Better Decisions</h5>
                    <p>Teacher:<strong>James Colins</strong></p>
                    <p>Price:strong <strong>$21.00</strong></p>
                    <button>View Course</button>
                </div>
            <!-- fourth card -->
                <div id="single_card">
                    <img src="" alt="">
                    <h5>Make Better Decisions</h5>
                    <p>Teacher:<strong>James Colins</strong></p>
                    <p>Price:strong <strong>$21.00</strong></p>
                    <button>View Course</button>
                </div>
            <!-- fifth card -->
                <div id="single_card">
                    <img src="" alt="">
                    <h5>Make Better Decisions</h5>
                    <p>Teacher:<strong>James Colins</strong></p>
                    <p>Price:strong <strong>$21.00</strong></p>
                    <button>View Course</button>
                </div>
            </div>
        </section>
        <!-- sixth section -->
        <section>
            <div id="sixth_left">
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
            <img src="" alt="">
        </section>
        <!-- seventh section -->
        <section>
            <img src="" alt="">
            <div id="seventh_right">
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



</style>