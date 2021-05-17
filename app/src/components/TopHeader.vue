<template>
    <v-app-bar
    absolute
    color="#fcb69f"
    dark
    shrink-on-scroll
    src="../assets/shirts-aroundabouts-laundry-full.jpg"
    scroll-target="#scrolling-techniques-2"
  >
    <template v-slot:img="{ props }">
      <v-img
        v-bind="props"
        gradient="to top right, rgba(19,84,122,.5), rgba(128,208,199,.8)"
      ></v-img>
    </template>

    <v-app-bar-nav-icon></v-app-bar-nav-icon>

    <v-app-bar-title>Around Abouts Laundry</v-app-bar-title>

    <v-spacer></v-spacer>

    <v-btn icon
    href="https://www.facebook.com/aroundabouts">
      <v-icon>mdi-facebook</v-icon>
    </v-btn>

    <v-btn icon
    href="https://www.google.co.uk/maps/place/Aroundabouts+Laundry/@50.3976214,-4.9255878">
      <v-icon >mdi-google-maps</v-icon>
    </v-btn>
  </v-app-bar>
</template>

<script>
export default {

  data: () => ({
    loading: false,
  }),
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
