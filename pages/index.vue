<template>
  <v-container fluid>
    <v-layout>
      <v-breadcrumbs
        style="padding-left: 0px; margin-top: 100px"
        large
        :items="items"
      />
    </v-layout>
    <div>
      <p class="caption" style="color: #43a047">
        <v-icon style="color: #43a047"> mdi-checkbox-marked-circle </v-icon>
        Preferred Merchant
      </p>
    </div>
    <p class="h2" style="font-size: 35px">Do Yan Seafood - Sumbersekar</p>
    <p class="body">Seafood, Snack</p>
    <v-row>
      <p class="body2">
        <v-icon style="color: gold"> mdi-star </v-icon>
        4.7
      </p>
      <p class="body2" style="margin-left: 80px">664.1 km</p>
    </v-row>
    <v-row>
      <p class="body2">Opening Hours</p>
      <p class="body2" style="margin-left: 80px">Today 13:00-22:00</p>
    </v-row>
  </v-container>
</template>

<script>
export default {
  name: "IndexPage",
  layout: "default",
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
