<template>
    <div id = "app">
        <Header title="VueJs" />
        <Profile :user="user" />
    </div>
</template>

<script>
  import Header from './components/Header';
  import Profile from './components/Profile';

  export default {
      name: 'App',
      components: {
        Header,
        Profile
      },
      data: function () {
        return {
                  user: {
                    name: "James",
                    image: require("./assets/spider-man.jpg")
                  }
               }
        }
   }
    
</script>

<style>
    body {
      background: #F3F3F3;
      margin: 0;
    }

    #app {
      font-family: Avenir, Helvetica, Arial, sans-serif;
      -webkit-font-smoothing: antialiased;
      -moz-osx-font-smoothing: grayscale;
      text-align: center;      
    }
</style>
