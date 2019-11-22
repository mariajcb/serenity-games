<template lang="html">
  <v-row no-gutters>
    <v-col
      v-for="n in 4"
      :key="n"
    >
      <v-card
        class="pa-2"
        max-height="300"
        tile
        outlined
      >
        <v-card-title>
          Title
        </v-card-title>
        <v-card-subtitle>
          Subtitle
        </v-card-subtitle>
        <v-card-text>
          This is some text
        </v-card-text>
        <v-card-actions>
          <v-btn
            text
          >
            Learn More
          </v-btn>
        </v-card-actions>
      </v-card>
    </v-col>
  </v-row>
</template>

<script>
export default {
  data () {
    return {

    }
  }
}
</script>

<style lang="css" scoped>
</style>
