<!--<template>
    <div class="col-xs-12 col-sm-6">
        <ul class="list-group">
            <li
                    class="list-group-item"
                    v-bind:key="index.id"
                    v-for="index in 5">
                Server #{{ index }}
            </li>
        </ul>
    </div>
</template>-->
<template>
    <!-- <v-app> -->
        <!-- <v-container fluid> -->
            <!-- <v-row>
                <v-col
                    cols="12"
                    sm="6"
                > -->
                    <v-card
                        class="mx-auto"
                        width="800"
                    >
                        <v-list-item-group
                            v-for="index in 5"
                            :key="index.id"
                        >
                            <v-list-item @click="changeStatus"> 
                                <v-list-item-content>
                                    Server #{{ index }}
                                </v-list-item-content>
                            </v-list-item>
                        </v-list-item-group>
                    </v-card>
                <!-- </v-col>
            </v-row> -->
        <!-- </v-container> -->
    <!-- </v-app> -->
</template>

<script>
    export default {
        data: function() {
          return {
            status: "Good"
          };
        },
        methods: {
            changeStatus: function() {
                this.status = "Bad";
            }
        }
    }
</script>

<style>

</style>>

