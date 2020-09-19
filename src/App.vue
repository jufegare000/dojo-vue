<template>
  <v-app>
    <Toolbar></Toolbar>
    <v-main>
      <Search v-on:searchResult="searchResult"></Search>
      <ImageList v-bind:items="items"/>
    </v-main>
  </v-app>
</template>

<script>
import Toolbar from "./components/Toolbar.vue";
import Search from "./components/Search.vue";
import ImageList from "./components/ImageList";

export default {
  name: 'App',

  components: {
    Toolbar,
    Search,
    ImageList
  },

  data: () => ({
    items: []
  }),
  methods: {
    searchResult(response){
      this.items=response;
    }
  }
};
</script>
