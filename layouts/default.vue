<template>
    <v-app dark>
        <v-content>
            <v-parallax src="/img/slides/2.png" class="fill-height" height="100%">
                <v-toolbar dark color="transparent" flat class="no-flex-toolbar">
                    <v-toolbar-title class="mx-5">
                        <span class="headline font-weight-bold">HS</span>
                        <span class="body-1 font-weight-light">GHANA</span>
                    </v-toolbar-title>
                    <v-spacer></v-spacer>
                    <v-btn text class="mx-5" nuxt to="/host/register">Host a traveler</v-btn>
                    <v-btn text class="mx-5" nuxt to="/login">Signup / Login</v-btn>
                    <v-btn icon class="mx-5">
                        <v-icon>menu</v-icon>
                    </v-btn>
                </v-toolbar>
                <v-spacer>
                    <nuxt/>
                </v-spacer>
            </v-parallax>
        </v-content>
    </v-app>
</template>

<script>
    export default {
        data() {
            return {
                clipped: false,
                drawer: false,
                fixed: false,
                items: [
                    {
                        icon: 'mdi-apps',
                        title: 'Welcome',
                        to: '/'
                    },
                    {
                        icon: 'mdi-chart-bubble',
                        title: 'Inspire',
                        to: '/inspire'
                    }
                ],
                miniVariant: false,
                right: true,
                rightDrawer: false,
                title: 'Vuetify.js'
            }
        }
    }
</script>

<style>
    * {
        /*font-family: Raleway !important;*/
    }

    .no-flex-toolbar {
        flex: none !important;
    }
</style>
