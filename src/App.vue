<template>
  <v-app>
    <TheNavigation/>
    <v-content>
      <v-container fluid>
        <Home />
      </v-container>
    </v-content>
  </v-app>
</template>

<script>
import Home from './views/Home'
import TheNavigation from './components/TheNavigation'

export default {
  name: 'App',
  components: {
    Home,
    TheNavigation
  }
}
</script>
