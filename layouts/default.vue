<template>
  <v-app>
    <v-main>
      <v-row style="padding-right: 150px; padding-left: 150px; margin-top: 0px">
        <Header />
        <Nuxt />
      </v-row>
      <Footer />
    </v-main>
  </v-app>
</template>

<script>
import Header from "~/components/Header.vue";
import Footer from "~/components/Footer.vue";

export default {
  name: "DefaultLayout",
};
</script>
