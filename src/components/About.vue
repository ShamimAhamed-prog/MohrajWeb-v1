<template>
  <v-container>
      <v-row>
        <div class="aboutimg">
          <v-col lg-6>
            <img src="./../assets/107.jpg" alt="107">
          </v-col>
        </div>
         <v-col lg-6>
                 <v-subheader class="about-des">
                        About Us
                    </v-subheader>
                    <br />
                      <br />
                    <p class="para">Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.</p>
                   <v-list>
                       <v-list-item> 
                           <v-icon color="success" class="mr-3">mdi-check-all</v-icon>
                           <v-list-item-subtitle>Contrary to popular belief.</v-list-item-subtitle>
                       </v-list-item>
                       <v-list-item> 
                           <v-icon color="success" class="mr-3">mdi-check-all</v-icon>
                           <v-list-item-subtitle>  The standard chunk of Lorem Ipsum used since the 1500s is reproduced below for those interested.</v-list-item-subtitle>
                       </v-list-item>
                           <v-list-item> 
                           <v-icon color="success" class="mr-3">mdi-check-all</v-icon>
                           <v-list-item-subtitle>Contrary to popular belief.</v-list-item-subtitle>
                       </v-list-item>
                       
                        <v-list-item> 
                           <v-icon color="success" class="mr-3">mdi-check-all</v-icon>
                           <v-list-item-subtitle>Contrary to popular belief.</v-list-item-subtitle>
                       </v-list-item>         
                       </v-list> 
                </v-col>      
      </v-row>
  </v-container>
</template>

<script>
export default {
         name:"About"
}
</script>

<style scoped>
</style>
