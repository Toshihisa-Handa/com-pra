<template>
  <v-app>
  <Header/>
  <Login/>
  <Home/>
  </v-app>
</template>

<script>
import Header from './views/Header';
import Login from './views/Login';
import Home from './views/Home';

export default {
  name: 'App',

  components: {
        Header,
        Login,
        Home,
  },

  data: () => ({
    //
  }),
};
</script>
