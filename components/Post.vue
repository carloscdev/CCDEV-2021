<template>
  <div class="my-10">
    <v-container>
      <h2 class="mb-5">Last Posts</h2>
      <v-row>
        <v-col v-for="n in 6" :key="n" class="col-12" md="4" sm="6">
          <v-hover v-slot:default="{ hover }">
            <v-img
              :src="`https://picsum.photos/500/300?image=${n * 5 + 10}`"
              :lazy-src="`https://picsum.photos/10/6?image=${n * 5 + 10}`"
              aspect-ratio="1"
              class="grey lighten-2"
              style="height:270px"
            >
              <v-expand-transition>
                <div
                  v-if="hover"
                  transition="scroll-y-reverse-transition"
                  class="d-flex flex-column transition-fast-in-fast-out white--text align-center justify-center"
                  style="height: 100%; background-color: rgba(0,0,0,0.9);"
                >
                  <h3 class="mb-3">
                    How use scss in nuxt js
                  </h3>
                  <v-btn class="mx-2" outlined dark small color="primary">
                    View Post
                    <v-icon dark right>
                      mdi-arrow-right-thick
                    </v-icon>
                  </v-btn>
                </div>
              </v-expand-transition>
            </v-img>
          </v-hover>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss">
.imageDetail {
  background-color: rgba($color: #121212, $alpha: 0.8);
  padding: 0 3rem;
}
.v-image__image:hover .imageDetail {
  display: flex;
}
</style>
