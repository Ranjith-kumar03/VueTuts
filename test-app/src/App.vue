<template>
  <!-- <nav>
    <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link>
  </nav> -->
  <!-- //<router-view/> -->
  <h1>please se my name {{greet}} {{name}}</h1>
  <!-- <h1 v-text="channel"></h1> -->
<h1 v-html="channel"></h1>
<h2 :id="headingId">Heading</h2>
<button :disabled="isDisabled">Hit Me</button>
<h2 class="underLine">See the Undeline</h2>
<h2 v-bind:class="status">We are in Danger</h2>
<h2 v-bind:class="ioOld ? 'old':'new'"> Movie Status</h2>
</template>
<script>
export default{
  

  data()
  {
    return{
        name:"Ranjith Kumar",
        greet:"hi Boss",
        channel:"<i>You Tube</i>",
        headingId:"heading",
        isDisabled:false,
        status:"danger",
        isOld:false,
    }
  }
}
</script>



<style scoped>


#headingId{
  background-color: blue;;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}
.underLine{
  text-decoration: underline;
}
.new{
  color: green;
}
.old{
  color: red;
}
</style>
