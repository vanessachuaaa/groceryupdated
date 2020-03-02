<template>
  <div class="headerStyle">
    <header>
        <h1>{{ msg }}</h1>
    </header>
    
  </div>
</template>

<script>
export default {
  
  data(){
    return{
        msg: 'Grocery List'
        }
  },
  //Lifecycle methods
  beforeCreate: function() {
     console.log("beforeCreate()")
     //alert("before create")
  },
  created: function() {
    console.log("created()")
    //alert("created")
  },
  beforeMount: function() {
    console.log("beforeMount()");

  },
  mounted: function() {
    setTimeout(function(){console.log("mounted()")}, 3000);
  }
  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
header{
    background:rgb(122, 63, 100);
    padding:10px;
    border-style: solid;
    border-color:black;
    border-width: 2px;
}
h1{
    color:ivory
}
</style>