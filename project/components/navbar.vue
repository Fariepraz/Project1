<template>
<div>
  
 
  <v-card
    
  >
    <v-toolbar color="green" >
      <v-app-bar-nav-icon color="white" @click="drawer=!drawer"></v-app-bar-nav-icon>

      <v-toolbar-title class="white--text"> Practice</v-toolbar-title>

      <v-spacer></v-spacer>
      <span class="white--text"> Log Out</span>
      <v-btn icon>
        <v-icon right>mdi-exit-to-app</v-icon>
      </v-btn>
    </v-toolbar>
    <v-navigation-drawer app v-model="drawer" color="grey lighten-3" >
      <v-list-item>
        <v-list-item-content>
        
        
        </v-list-item-content>
      </v-list-item>
      <v-list
        dense
        nav
      >
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
  
  </v-card>
   </div> 
</template>

<script>
  export default {
    data(){
        return{
            drawer: false,
             items: [
          { title: 'Dashboard', icon: 'mdi-view-dashboard' },
          { title: 'Photos', icon: 'mdi-image' },
          { title: 'About', icon: 'mdi-help-box' },
        ],
        right: null,
        
        }
    }
  }
</script>