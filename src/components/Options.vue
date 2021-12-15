<template>
    <ul>
        <!-- Buttons -->
        <li>{{details.name}}</li>
        <i :class= details.img></i>
    </ul>
</template>

<script>
export default {
  name:"Options",
  props: {
      details:Object
  }
}
</script>

<style>

ul{
    list-style-type: none;
    display: flex;
    align-items: center;
}

i{
    padding-left: 10px;
    padding-right: 30px;
    font-size:10px;
}

</style>