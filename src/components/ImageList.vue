<template>
    <v-container>
        <v-row>
            <v-col v-for="item in items.hits" v-bind:key="item.id">
                <v-card>
                    <img class="ma-2" :src="item.previewURL" alt />
                    <v-card-title>
                        {{item.user}}
                    </v-card-title>
                </v-card>
            </v-col>
        </v-row>
    </v-container>
</template>
<script>
export default {
    name: "imageList",
    props: ["items"]
}
</script>