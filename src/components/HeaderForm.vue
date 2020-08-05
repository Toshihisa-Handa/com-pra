<template>

  <div>
    <v-app-bar
      
      color="pink lighten-2"
      dense
      dark
    >
      <v-app-bar-nav-icon @click.stop="drawer = !drawer"></v-app-bar-nav-icon>
      <v-toolbar-title>Life Flower</v-toolbar-title>
      <v-spacer></v-spacer>

     <router-link active-class="current" v-bind:to="{ name: 'Top'}">
      <v-btn icon>
        <v-icon>mdi-home</v-icon>
      </v-btn>
     </router-link>

<router-link active-class="current" v-bind:to="{ name: 'ShopList'}">
      <v-btn icon>
        <v-icon>mdi-flower-tulip</v-icon>
      </v-btn>
     </router-link>

      <router-link active-class="current" v-bind:to="{ name: '#'}">
      <v-btn icon>
        <v-icon>mdi-heart</v-icon>
      </v-btn>
     </router-link>

      <router-link active-class="current" v-bind:to="{ name: '#'}">
      <v-btn icon>
        <v-icon>mdi-magnify</v-icon>
      </v-btn>
     </router-link>

      <router-link active-class="current" v-bind:to="{ name: 'Form'}">
      <v-btn icon>
        <v-icon>mdi-file-document-outline</v-icon>
      </v-btn>
     </router-link>

      <router-link active-class="current" v-bind:to="{ name: 'Login'}">
      <v-btn icon>
        <v-icon>mdi-login</v-icon>
      </v-btn>
     </router-link>

      <router-link active-class="current" v-bind:to="{ name: 'Top'}">
      <v-btn icon>
        <v-icon>mdi-logout</v-icon>
      </v-btn>
     </router-link>

      <router-link active-class="current" v-bind:to="{ name: 'Top'}">
      <v-btn icon>
        <v-icon>mdi-account-plus</v-icon>
      </v-btn>
     </router-link>
  
    </v-app-bar>
  </div>
      
   
</template>
<style scoped>
a {
  text-decoration: none;
}
.current .v-btn--icon .v-icon {
  color: #ff80ab;
}
</style>

<script>
  export default {
    data () {
      return {
        drawer: null,
        items: [
          { title: 'Home', icon: 'mdi-home' },
          { title: 'Flower-List', icon: 'mdi-flower-tulip' },
        ],
      }
    },
  }
</script>