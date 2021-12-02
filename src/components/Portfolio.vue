<template>
<v-container>
    <v-row justify="center">
        <v-col lg="12" class="text-center">
            <v-subheader class="text-h4 justify-center">Portfolio</v-subheader>
            <p>Hello This is company Portfolio</p>
        </v-col>
        <v-col lg="3">
            <div class="text-center">

                <v-chip class="ma-2" color="primary">
                    Digital Marketing
                </v-chip>

                <v-chip class="ma-2" color="red" text-color="white">
                    Reseller
                </v-chip>

                <v-chip class="ma-2" color="green" text-color="white">
                    E-commerce
                </v-chip>
                 <v-chip class="ma-2" color="green" text-color="white">
                    Nothing
                </v-chip>
            </div>
        </v-col>
    </v-row>
</v-container>
</template>

<script>
export default {
    name: "Portfolio"
}
</script>

<style>

</style>
