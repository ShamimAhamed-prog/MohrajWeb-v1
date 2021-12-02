<template>
<v-container>
    <v-row justify="center">
        <v-col lg="12" class="text-center">
            <v-subheader class="text-h4 justify-center">Portfolio</v-subheader>
            <p>Hello This is company Portfolio</p>
        </v-col>
        <v-col lg="12">
            <div class="text-center">

                <v-chip  @click= "activePortfolio = 'digitalmarketing'"  class="mx-5" :color="activePortfolio == 'digitalmarketing'?'success':'' " >
                    Digital Marketing
                </v-chip>

                <v-chip  @click= "activePortfolio= 'reseller'"  class="mx-5" :color="activePortfolio == 'reseller'?'success':'' " >
                    Reseller
                </v-chip>

                <v-chip  @click= "activePortfolio= 'ecommerce'" class="mx-5" :color="activePortfolio == 'ecommerce'?'success':'' " >
                    E-commerce
                </v-chip>
               
            </div>
        </v-col>
              <slot v-if="activePortfolio=='digitalmarketing'">
                    <v-col lg="3" v-for="(web,webindex) in webApps" :key="webindex" >
                    <v-card>
                        <v-img 
                        :src="web.image" 
                        class="white--text align-end"
                        gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)" 
                        height="200px"
                        >
                            <v-card-title>{{web.title}}</v-card-title>
                        </v-img>
                    </v-card>
                </v-col>
              </slot>
    </v-row>
</v-container>
</template>

<script>
export default {
    name: "Portfolio",
     data(){
        return{
            activePortfolio:'digitalmarketing',
            webApps:[
                {title:'Digital Marketing', image: './../assets/digital.jpg'},
                {title:'Reseller', image:'./../assets/reseller.png'},
                {title:'E-commerce', image:'./../assets/ecommerce.png'}
            ]

        }
    }
}
</script>

<style>

</style>
