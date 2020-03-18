<template>
    <v-container class="fill-height">
        <v-layout class="content-wrapper" column justify-space-between="">
            <div class="d-flex flex-column">
                <p class="py-0 my-0 display-1 font-weight-bold text-left">Welcome Back</p>
            </div>
            <v-row style="flex: none;">
                <v-col class="filter pb-0">
                    <v-text-field label="EMAIL OR USERNAME" filled type="email" dark></v-text-field>
                </v-col>
                <v-spacer></v-spacer>
                <v-col class="filter pb-0">
                    <v-text-field label="PASSWORD" filled type="password" dark></v-text-field>
                </v-col>
            </v-row>
            <div class="d-flex">
                <v-btn dark text>I do not have an account</v-btn>
                <v-spacer></v-spacer>
                <v-btn color="primary" dark large>Log in</v-btn>
            </div>
        </v-layout>
    </v-container>
</template>

<script>
    export default {
        components: {}
    }
</script>

<style scoped>

    .content-wrapper {
        padding-right: 100px !important;
        padding-left: 100px !important;
        max-height: 700px !important;
        width: 100%;
    }

    .h-curve {
        border-top-right-radius: 100px !important;
        border-bottom-left-radius: 100px !important;
    }

    .filter {
        max-width: 600px;
    }
</style>
