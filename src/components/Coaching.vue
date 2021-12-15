<template>
    <div id="event_card">
        <div id="event">
            <h4>Coaching session</h4>
            <p> {{lesson.date}}</p>
            <p>Lorem ipsum dolor sit amet consectetur <br>
            adipisicing elit, sed do eiusmod tempor[...]</p>
        </div>
        <button id="event_button_second"> + find more </button>
    </div>
</template>

<script>
export default {
name:"Coaching",
    props: {
    lesson: Object
  }
}
</script>

<style>

#event_card{
    display: flex;
    flex-direction: column;
}

#event{
    padding: 40px 20px;
    background-color:#ffffff;
    border-radius: 10px;
    margin: 15px;
    box-shadow: 2px 0px 10px #949393;
}

#event p{
    padding:10px;
    color: #868892;
}

#event h2{
    color:#3d404f;
}

#event_button_second{
    background-color: #e56768;
    border-radius: 40px;
    border:none;
    padding: 10px;
    width:120px;
    margin: 0 auto;
    margin-top:-30px;
    color: white;
    box-shadow: 2px 0px 10px #e56768;
}

</style>