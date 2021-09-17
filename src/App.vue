<template>
  <Header text="Welcome"/>
  <h2>See also other Front End JS Frameworks</h2>
  <Slots :tasks="tasks"/>
</template>

<script>
import Slots from './components/Slots.vue'
import Header from './components/Header.vue'


export default {
  name: 'App',
  components: {
    Slots,
    Header
  },
  data(){
    return {
      tasks:[
        {id:1,
         img:"https://cdn.freelogovectors.net/wp-content/uploads/2018/12/react_logo.png",
         name:"React",
         desc:"Lorem ipsum dolor sit amet, consectetur adipiscing elit."},

        {id:2,
        img:"https://angular.io/assets/images/logos/angularjs/AngularJS-Shield.svg",
        name:"Angular",
        desc:"Lorem ipsum dolor sit amet, consectetur adipiscing elit."},

        {id:3,
        img:"https://emberjs.com/images/brand/ember-tomster-lockup-4c.svg",
        name:"Ember",
        desc:"Lorem ipsum dolor sit amet, consectetur adipiscing elit."},

        {id:4,
        img:"https://www.indianlancer.com/wp-content/uploads/2019/03/backbone.js-icon.png",
        name:"Backbone",
        desc:"Lorem ipsum dolor sit amet, consectetur adipiscing elit."},]

    }
  }
}
</script>

<style>

  h3 {
  margin: 40px 0 0;
}

  h1,h2{
    font-family: 'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial, sans-serif;
  }

  h1{
    font-size: 4rem;
  }

  h2{
    font-size: 2rem;
  }

  #app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

</style>
