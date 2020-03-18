<template>
    <v-container class="fill-height" fluid>
        <v-layout class="content-wrapper" fill-height="" justify-space-between="" row>
            <v-card class="search-box" color="#ffffff80" width="100%">
                <v-toolbar height="100">
                    <v-layout align-end="" fill-height="" row>
                        <v-col class="filter pb-0">
                            <v-text-field append-icon="location_searching" filled label="WHERE TO"
                                          single-line></v-text-field>
                        </v-col>
                        <v-spacer></v-spacer>
                        <v-col class="filter pb-0">
                            <v-text-field append-icon="date_range" filled label="ARRIVAL" type="date"></v-text-field>
                        </v-col>
                        <v-col class="filter pb-0">
                            <v-text-field filled label="DEPARTURE" prepend-inner-icon="date_range"
                                          type="date"></v-text-field>
                        </v-col>
                        <v-col class="filter pb-0">
                            <v-slider prepend-icon="people" thumb-label="always" value="45"></v-slider>
                        </v-col>
                    </v-layout>
                </v-toolbar>
                <v-row class="spacer">
                    <v-col cols="8">
                        <v-row class="px-3">
                            <v-col cols="4" v-for="i in 12" :key="i">
                                <SearchItem/>
                            </v-col>
                        </v-row>
                    </v-col>
                    <v-col col="4"></v-col>
                </v-row>
            </v-card>
        </v-layout>
    </v-container>
</template>

<script>
    import SearchItem from "../components/SearchItem";

    export default {
        name: "search",
        components: {SearchItem}
    }
</script>

<style>
    .content-wrapper {
        padding-right: 100px !important;
        padding-left: 100px !important;
    }

    .search-box {
        border-top-left-radius: 50px;
        border-top-right-radius: 50px;
        overflow: hidden;
    }

    .filter {
        max-width: 300px;
    }

</style>
