<template>
  <v-app>
    <TheNavigation/>
    <v-content>
      <v-container fluid>
        <Home />
      </v-container>
    </v-content>
    <TheFooter />
  </v-app>
</template>

<script>
import Home from './views/Home'
import TheNavigation from './components/global/TheNavigation'
import TheFooter from './components/global/TheFooter'

export default {
  name: 'App',
  components: {
    Home,
    TheNavigation,
    TheFooter
  }
}
</script>
