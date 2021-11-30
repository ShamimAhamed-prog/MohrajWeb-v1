<template>
  <v-container>
      <v-row>
          <v-col lg="6">
                <h1 class="intro-text">Welcome To Moharaj Ltd.</h1>
                <p class="description">
                    Hello Everyone.We are from Moharaj ltd for serving you and our nation.
                </p>
                <!-- <v-btn color="success"  class="white--text"  rounded>Visit Us</v-btn> -->
                    <v-btn color="indigo"  class="white--text" rounded>
                    <v-icon>mdi-play-circle</v-icon> Watch Our Organisation</v-btn>
          </v-col>
          <div class="frontimg">
          <v-col lg="6">
              <img  src="./../assets/front.jpg" alt="front">
          </v-col>
          </div>
      </v-row>
  </v-container>
</template>

<script>
    export default {
        name:"Home"
    }
</script>
<style scoped>

</style>