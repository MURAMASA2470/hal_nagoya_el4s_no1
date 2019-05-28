<template>
    <v-layout>
    <v-flex>
        <h2 class="text-xs-center">title</h2>
        <v-layout row wrap align-center justify-space-around>
            <v-flex xs12 sm4 pa-2 v-for="n in 6" :key="n">

            <v-card>
                <v-img
                src="https://cdn.vuetifyjs.com/images/cards/desert.jpg"
                aspect-ratio="2.75"
                ></v-img>

                <v-card-title primary-title>
                <div>
                    <h3 class="headline mb-0">Kangaroo Valley Safari</h3>
                    <div> text </div>
                </div>
                </v-card-title>

                <v-card-actions>
                <v-btn flat color="orange">Share</v-btn>
                </v-card-actions>
            </v-card>

            </v-flex>

        </v-layout>
    </v-flex>
    </v-layout>
</template>
