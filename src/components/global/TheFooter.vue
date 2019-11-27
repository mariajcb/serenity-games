<template lang="html">
  <v-footer padless>
    <v-col
      class="text-center"
      cols="12"
    >
      ©{{ new Date().getFullYear() }} — <strong>Serenity Games</strong>
    </v-col>
  </v-footer>
</template>

<script>
export default {
  data: () => ({
    icons: [
      'mdi-facebook',
      'mdi-twitter',
      'mdi-instagram'
    ]
  })
}
</script>

<style lang="css" scoped>
</style>
