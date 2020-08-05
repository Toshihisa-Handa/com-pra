<template>
 <v-sheet
    height="400"
    class="overflow-hidden"
    style="position: relative;"
  >
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
     <v-navigation-drawer
      v-model="drawer"
      absolute
      temporary
    >
      <v-list-item>
        <v-list-item-avatar>
          <v-img src="https://randomuser.me/api/portraits/men/78.jpg"></v-img>
        </v-list-item-avatar>

        <v-list-item-content>
          <v-list-item-title>John Leider</v-list-item-title>
        </v-list-item-content>
      </v-list-item>

      <v-divider></v-divider>

      <v-list dense>

        <v-list-item
          v-for="item in items"
          :key="item.title"
          link
        >
          <v-list-item-icon>
            <v-icon>{{ item.icon }}</v-icon>
          </v-list-item-icon>

          <v-list-item-content>
            <v-list-item-title>{{ item.title }}</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>
  </div>
      
     </v-sheet>

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