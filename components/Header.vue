<template>
  <v-app app>
    <v-app-bar
      elevation="0"
      color="white"
      app
      fixed
      flat
      style="padding-right: 150px; padding-left: 150px; margin-top: 15px"
    >
      <!-- <v-layout> -->
      <v-flex height="20px">
        <v-img
          height="130px"
          width="130px"
          src="/images/grabfood.png"
          contain
        />
      </v-flex>
      <!-- <v-btn outlined style="margin-right: 10px">
        <v-icon> mdi-cart </v-icon>
      </v-btn> -->
      <!-- </v-layout> -->

      <v-text-field
        style="margin-top: 25px; margin-right: 500px"
        placeholder="Type youre Location"
        dense
        prepend-inner-icon="mdi-map-marker"
        outlined
        elevation="1"
      ></v-text-field>
      <v-btn outlined style="margin-right: 10px; margin-top: 15px">
        <v-icon> mdi-cart </v-icon>
      </v-btn>
      <v-btn class="text-none" style="margin-top: 15px" outlined> Login/Sign Up </v-btn>
    </v-app-bar>
  </v-app>
</template>


<script>
export default {
  name: "DefaultLayout",
  data() {
    return {
      title: "Vuetify.js",
      items: [
        {
          text: "Home",
          disabled: false,
          href: "breadcrumbs_dashboard",
        },
        {
          text: "Restaurant",
          disabled: false,
          href: "breadcrumbs_link_1",
        },
        {
          text: "Do Yan Seafood - Sumbersekar",
          disabled: true,
          href: "breadcrumbs_link_2",
        },
      ],
    };
  },
};
</script>