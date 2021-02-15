<template>
  <div>
    <v-footer :absolute="!fixed" app>
      <v-container>
        <v-row class="d-flex align-center">
          <v-col class="col-12">
            <span>&copy; {{ new Date().getFullYear() }}</span>
          </v-col>
        </v-row>
      </v-container>
    </v-footer>
  </div>
</template>

<script>
export default {
  data() {
    return {
      fixed: false
    };
  }
};
</script>

<style></style>
