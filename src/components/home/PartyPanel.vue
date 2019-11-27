<template lang="html">
  <v-card
    class="mx-auto"
    color="black"
  >

    <v-container>
      <v-row dense>

        <v-col
          cols="12"
        >
          <v-card
            dark
            color="black"
            class="py-7"
          >
            <v-avatar
              class="ma-3 d-sm-none"
              size="300"
              tile
            >
              <v-img src="@/assets/party-panel-fireworks.png"></v-img>
            </v-avatar>
            <div class="d-flex flex-no-wrap justify-space-between">
              <div>
                <v-card-title
                  class="display-4 mb-7 font-weight-black"
                >Party?</v-card-title>
                <v-card-subtitle class="headline">You can get catering, rent games, or even book your own personal DM, so you can focus on the important part: having fun!</v-card-subtitle>
              </div>
              <v-avatar
                class="ma-3 d-none d-sm-flex"
                size="300"
                tile
              >
                <v-img src="@/assets/party-panel-fireworks.png"></v-img>
              </v-avatar>
            </div>
            <v-card-actions>
                <v-btn
                  width="200"
                  height="55"
                  large
                  light
                  color="amber"
                  class="font-weight-black">Book it</v-btn>
            </v-card-actions>
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
