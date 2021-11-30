<template>
<v-row no-gutters>
    <v-app-bar   v-for="n in 3"
          :key="n"
      app
      color="white"
      light
      elevation="6"
      elevate-on-scroll
    >  
       <v-toolbar-title>
        <img src="./../assets/logo.png">
       </v-toolbar-title>
       <v-spacer />
       <v-list class="d-flex align-center">
         <v-list-item link v-for="(menu,index) in menus" :key="index" :to="menu.route">
          <v-list-item-title>
                      {{menu.title}}
          </v-list-item-title>
         </v-list-item>
         <v-btn text>
           <v-icon>
             mdi-magnify
           </v-icon>
         </v-btn>
         <v-btn outlined color="success">Get Started</v-btn>
       </v-list>

    </v-app-bar>
  </v-row>

</template>
<script>
export default{
    name:"Header",

  data: () => ({
    menus:[
      {title:'Home', route:'Home'},
      {title:'About', route:'About'},
      {title:'Portfolio', route:'Portfolio'},
      {title:'Projects', route:'projects'},
      {title:'Contact', route:'contact'}
    ]
  })
}
</script>
<style scoped>

</style>