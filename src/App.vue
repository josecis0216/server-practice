<template>
    <v-app>
        <div class="container">
            <app-header></app-header>
            <hr>
            <v-container fluid>
                <v-row>
                    <v-col cols="12" sm="6">
                        <app-servers></app-servers>
                    </v-col>
                    <v-col cols="12" sm="6">
                        <app-server-details></app-server-details>
                    </v-col>
                </v-row>
            </v-container>
            <hr>
            <app-content></app-content>
            <hr>
            <app-footer></app-footer>
        </div>
        </v-app>
</template>

<script>
    import Header from './components/Header.vue';
    import Footer from './components/Footer.vue';
    import Servers from './components/Servers.vue';
    import ServerDetails from './components/ServerDetails.vue';
    import Content from './components/Content.vue';

    export default {
        data: () => {
          return {
            status: "Good"
          }
        },
        components: {
            'app-header': Header,
            'app-servers': Servers,
            'app-server-details': ServerDetails,
            'app-content': Content,
            'app-footer': Footer
        }
    }
</script>

<style>

</style>
