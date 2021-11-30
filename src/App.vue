<template>
<v-app>
    <Header />
    <v-main>
        <Slider />
        <Home />
        <About />
        <br />
              <br />
                    <br />
        <Portfolio />
    </v-main>
</v-app>
</template>

<script>
import Header from "./components//Header.vue"
import Home from "./components/Home.vue"
import About from "./components/About.vue"
import Portfolio from "./components/Portfolio.vue"
import Slider from './components/Slider.vue'

export default {
    name: 'App',

    components: {
        Header,
        Slider,
        Home,
        About,
        Portfolio,

    },

};
</script>
