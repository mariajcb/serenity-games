<template>
  <v-app>
    <TheNavigation/>
    <v-content>
      <v-container fluid>
        <router-view />
      </v-container>
    </v-content>
    <TheFooter />
  </v-app>
</template>

<script>
import TheNavigation from './components/global/TheNavigation'
import TheFooter from './components/global/TheFooter'

export default {
  name: 'App',
  components: {
    TheNavigation,
    TheFooter
  }
}
</script>

<style lang="css">
.v-image__image {
  opacity: 0.6!important;
}
</style>
