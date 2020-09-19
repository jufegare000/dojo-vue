<template>
  <v-card class="overflow-hidden">
    <v-app-bar
      absolute
      color="#fcb69f"
      dark
      shrink-on-scroll
      src="https://wearethemutantsdotcom.files.wordpress.com/2018/01/watm-motown-sounds.jpg"
      scroll-target="#scrolling-techniques-2"
    >
      <template v-slot:img="{ props }">
        <v-img
          v-bind="props"
          gradient="to top right, rgba(19,84,122,.5), rgba(128,208,199,.8)"
        ></v-img>
      </template>

      <v-app-bar-nav-icon></v-app-bar-nav-icon>

      <v-toolbar-title>My Gallery</v-toolbar-title>

      <v-spacer></v-spacer>

    </v-app-bar>
    <v-sheet
      id="scrolling-techniques-2"
      class="overflow-y-auto"
      max-height="600"
    >
      <v-container style="height: 125px;"></v-container>
    </v-sheet>
  </v-card>
</template>
<script>
export default {
    name: 'Toolbar'
}
</script>