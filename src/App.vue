<template>
  <v-app>
  <Header/>
  <!-- <Login/> -->
  <!-- <Home/>
  <Top/> 
  <ShopList/> 
  <Form/>  -->
  <router-view/>
  </v-app>
</template>

<script>
import Header from './views/Header';
// import Login from './views/Login';
// import Home from './views/Home';
// import Top from './views/Top';
// import ShopList from './views/ShopList';
// import Form from './views/Form';

export default {
  name: 'App',

  components: {
        Header,
        // Login,
        // Home,
        // Top,
        // ShopList,
        // Form,
  },

  data: () => ({
    //
  }),
};
</script>
