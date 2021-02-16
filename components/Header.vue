<template>
  <v-container column justify-center align-center>
    <v-row style="min-height: 400px;" class="d-flex align-center">
      <v-col class="col-sm-6 col-md-8">
        <h1 style="font-size: 3.5rem">CARLOS CÓRDOVA</h1>
        <span class="text--secondary my-3 d-block">
          {{ $t("message.des") }}</span
        >
        <br />
        <!-- <v-btn outlined color="primary">
          View Posts
        </v-btn> -->
        <br />
        <nuxt-link :to="switchLocalePath('en')">English</nuxt-link> <br />
        <nuxt-link :to="switchLocalePath('es')">Español</nuxt-link>
      </v-col>
      <v-col class="col-6 col-md-4"> </v-col>
    </v-row>
    <v-spacer></v-spacer>
  </v-container>
</template>

<script>
export default {
  data() {
    return {};
  }
};
</script>

<style></style>
