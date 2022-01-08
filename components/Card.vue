<template>
  <v-card class="mx-auto" max-width="450" hover=true>
    <v-list-item three-line>
      <v-list-item-avatar
        tile
        size="100"
        color="grey"
        rounded="true"
        border-radius="5px"
        class="rounded-lg"
      >
        <v-img
          class="white--text align-end"
          height="200px"
          src="https://cdn.vuetifyjs.com/images/cards/docks.jpg"
        >
        </v-img
      ></v-list-item-avatar>
      <v-list-item-content>
        <div class="text-body">
          Seo Goo Lalapan Ikan Laut Bakar/Goreng (Banyak Pilihan Ikan)
        </div>
        <!-- <v-list-item-title class="text-h5 mb-1">
          Seo Goo Lalapan Ikan Laut Bakar/Goreng (Banyak Pilihan
          Ikan)</v-list-item-title
        > -->
        <v-list-item-subtitle
          >Ikan Laut+Nasi dibakar dengan bumbu Bikin Doyan</v-list-item-subtitle
        >
      </v-list-item-content>
    </v-list-item>

    <!-- <v-card-subtitle class="pb-0"> Number 10 </v-card-subtitle> -->

    <!-- <v-card-text class="text--primary">
      <div>Whitehaven Beach</div>

      <div>Whitsunday Island, Whitsunday Islands</div>
    </v-card-text> -->

    <v-card-actions>
      <v-spacer></v-spacer>
      <v-btn color="green" small elevation="2">
        <v-icon color="white"> mdi-plus </v-icon>
      </v-btn>
    </v-card-actions>
  </v-card>
</template>

<script>
export default {};
</script>