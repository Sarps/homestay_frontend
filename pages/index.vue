<template>
    <v-container class="fill-height" fluid>
        <v-layout align-center="" class="content-wrapper" fill-height="" justify-space-between="" row>
            <div class="d-flex flex-column">
                <v-btn :key="i" class="my-5" icon large v-for="i in 4">
                    <v-icon large>all_out</v-icon>
                </v-btn>
            </div>
            <div class="d-flex flex-column">
                <div class="text-container">
                    <p class="py-0 my-0 display-4">CONVENIENCE</p>
                    <v-divider class="underline" color="white"></v-divider>
                </div>
                <div class="text-container">
                    <p class="py-0 my-0 display-1 text-center" style="letter-spacing: 3px !important;">NEVER FIND
                        YOURSELF WANTING</p>
                    <v-divider class="underline" color="white"></v-divider>
                </div>
            </div>
            <div>
                <v-card class="h-curve pa-8" height="700" width="550">
                    <v-card-title class="display-1 font-weight-bold pb-12 px-3">
                        BOOK A TRIP TO GHANA
                    </v-card-title>
                    <v-card-text>
                        <v-row class="pb-6">
                            <v-col cols="12">
                                <v-text-field append-icon="location_searching" filled
                                              hint="You can use the location picker to the right" label="WHERE TO"
                                              persistent-hint></v-text-field>
                            </v-col>
                        </v-row>

                        <v-row>
                            <v-col cols="12">
                                <v-subheader class="pl-0">HOW MANY</v-subheader>
                            </v-col>
                            <v-col class="pr-0" cols="6">
                                <v-text-field append-icon="date_range" filled label="ARRIVAL" outlined
                                              type="date"></v-text-field>
                            </v-col>
                            <v-col class="pl-0" cols="6">
                                <v-text-field filled label="DEPARTURE" outlined prepend-inner-icon="date_range"
                                              type="date"></v-text-field>
                            </v-col>
                        </v-row>

                        <v-row>
                            <v-col cols="12">
                                <v-subheader class="pl-0">HOW MANY</v-subheader>
                                <v-slider
                                    prepend-icon="people"
                                    thumb-label="always"
                                    value="45"
                                ></v-slider>
                            </v-col>
                        </v-row>

                        <v-row>
                            <v-col cols="12" class="d-flex justify-end">
                                <v-btn class="h-curve-btn right" color="primary" href="" nuxt to="/search">Search</v-btn>
                            </v-col>
                        </v-row>

                    </v-card-text>
                </v-card>
            </div>
        </v-layout>
    </v-container>
</template>

<script>
    export default {
        components: {}
    }
</script>

<style>

    .content-wrapper {
        padding-right: 100px !important;
        padding-left: 100px !important;
    }

    .h-curve {
        border-top-right-radius: 100px !important;
        border-bottom-left-radius: 100px !important;
    }

    .h-curve-btn {
        border-top-right-radius: 15px !important;
        border-bottom-left-radius: 15px !important;
    }

    .text-container {
        overflow: hidden;
    }

    .underline {
        margin-top: -8px;
    }

    .underline:first-of-type {
        margin-bottom: 20px;
    }
</style>
