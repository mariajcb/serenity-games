<template>
  <v-app>
    <NavDrawer :drawer="drawer"/>
    <v-app-bar
      app
      color="grey darken-4"
    >
      <v-app-bar-nav-icon  @click.stop="drawer = !drawer"></v-app-bar-nav-icon>
      <v-toolbar-title
        class="mt-2 hidden-sm-and-down"
        style="font-size: 1.75rem; font-family: Papyrus;">
          Serenity Games
      </v-toolbar-title>
      <v-spacer></v-spacer>

      <v-btn
        href="https://github.com/vuetifyjs/vuetify/releases/latest"
        target="_blank"
        icon
        class="mr-2"
      >
        <v-icon>mdi-phone</v-icon>
      </v-btn>
      <v-btn
        href="https://github.com/vuetifyjs/vuetify/releases/latest"
        target="_blank"
        icon
        class="mr-2"
      >
        <v-icon>mdi-calendar</v-icon>
      </v-btn>
      <v-btn
        href="https://github.com/vuetifyjs/vuetify/releases/latest"
        target="_blank"
        icon
        class="mr-2"
      >
        <v-icon>mdi-facebook</v-icon>
      </v-btn>
    </v-app-bar>

    <v-content>
      <v-container fluid>
        <Home />
      </v-container>
    </v-content>
  </v-app>
</template>

<script>
import Home from './views/Home'
import NavDrawer from './components/NavDrawer'

export default {
  name: 'App',
  components: {
    Home,
    NavDrawer
  },
  data () {
    return {
      drawer: false
    }
  }
}
</script>
