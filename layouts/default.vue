<template>
  <v-app>
    <v-main>
      <v-layout
        style="padding-right: 150px; padding-left: 150px; margin-top: 0px"
      >
        <Header />
        <Nuxt />
      </v-layout>
    </v-main>
  </v-app>
</template>

<script>
import Header from "~/components/Header.vue";

export default {
  name: "DefaultLayout",
};
</script>
