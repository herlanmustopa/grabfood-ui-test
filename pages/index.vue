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
      <p class="h2" style="font-size: 35px">Do Yan Seafood - Sumbersekar</p>
      <p class="body">Seafood, Snack</p>
      <v-row style="margin-left: 0px">
        <p class="body2">
          <v-icon style="color: gold"> mdi-star </v-icon>
          4.7
        </p>
        <p class="body2" style="margin-left: 80px">664.1 km</p>
      </v-row>
      <v-row style="margin-left: 0px">
        <p class="body2">Opening Hours</p>
        <p class="body2" style="margin-left: 80px">Today 13:00-22:00</p>
      </v-row>
      <v-row style="margin-left: 0px">
        <p class="body2">
          <v-icon style="color: green"> mdi-tag </v-icon>
        </p>
        <p class="body2" style="margin-left: 10px">HEMAT40 40% | HEMAT35 35%</p>
        <p class="body2" style="margin-left: 80px">Today 13:00-22:00</p>
      </v-row>
      <v-row style="margin-left: 0px">
        <p class="body2">
          <v-icon style="color: grey"> mdi-information </v-icon>
        </p>
        <p class="body2" style="margin-left: 10px">
          Order fee of Rp3.000 applies for this restaurant.
        </p>
      </v-row>
    </div>
    <!-- <v-card> -->
    <v-tabs elevation=" 1" v-model="tab" style="margin-left: -15px">
      <v-tab v-for="item in itemstab" :key="item.tab" color="green">
        {{ item.tab }}
      </v-tab>
    </v-tabs>

    <v-tabs-items v-model="tab">
      <v-tab-item v-for="item in itemstab" :key="item.tab">
        <v-card flat>
          <v-card-text>{{ item.content }}</v-card-text>
        </v-card>
      </v-tab-item>
    </v-tabs-items>
    <!-- </v-card> -->
    <p class="h6" style="margin-left: 10px">Aigo</p>
    <v-row>
      <v-col cols="4" sm="6" md="4">
        <Card />
      </v-col>
      <v-col cols="4" sm="6" md="4">
        <Card />
      </v-col>
      <v-col cols="4" sm="6" md="4">
        <Card />
      </v-col>
      <v-col cols="4" sm="6" md="4">
        <Card />
      </v-col>
      <v-col cols="4" sm="6" md="4">
        <Card />
      </v-col>
      <v-col cols="4" sm="6" md="4">
        <Card />
      </v-col>
      <!-- <v-col cols="4" sm="6" md="8">
        <Card />
      </v-col>
      <v-col cols="4" sm="6" md="8">
        <Card />
      </v-col> -->
    </v-row>

    <v-container></v-container>
  </v-container>
</template>

<script>
import Card from "~/components/Card.vue";

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
      tab: null,
      itemstab: [
        { tab: "Aigo", content: "Tab 1 Content" },
        { tab: "Chingu", content: "Tab 2 Content" },
        { tab: "Seeramon Ikan", content: "Tab 3 Content" },
        { tab: "Samjang Gani (Extra Pedas)", content: "Tab 4 Content" },
        { tab: "Sea Monster", content: "Tab 5 Content" },
        { tab: "Omo", content: "Tab 6 Content" },
        { tab: "Saranghayeo", content: "Tab 7 Content" },
        { tab: "Chaeso", content: "Tab 8 Content" },
        { tab: "Drink", content: "Tab 9 Content" },
        { tab: "Addon", content: "Tab 10 Content" },
      ],
    };
  },
};
</script>
