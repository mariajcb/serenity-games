<template lang="html">
  <v-card
    class="mx-auto"
    color="#85450A"
  >
    <v-container>
      <v-row dense>
        <v-col
          cols="12"
        >
          <v-card
            dark
            color="#85450A"
            flat
            class="py-7"
          >
            <div class="d-flex flex-no-wrap justify-space-between">
              <v-avatar
                class="ma-3"
                size="125"
                circle
              >
                <v-img src="@/assets/bio-photo.jpg"></v-img>
              </v-avatar>
              <div>
                <v-card-title
                  class="headline mb-1 font-weight-black"
                >About the Captain</v-card-title>
                <v-card-subtitle class="subtitle-1">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</v-card-subtitle>
                <v-card-actions>
                    <v-btn
                      text
                      class="font-weight-black"
                      to="/crew">Meet the crew
                      <v-icon>
                        mdi-chevron-right
                      </v-icon>
                    </v-btn>
                </v-card-actions>
              </div>
            </div>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </v-card>
</template>

<script>
export default {
}
</script>

<style lang="css" scoped>
</style>
