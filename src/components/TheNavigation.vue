<template lang="html">
  <div>
    <v-navigation-drawer
      color="grey darken-4"
      v-model="drawer"
      left
      dark
      app>
        <v-list-item>
          <v-list-item-content>
            <v-list-item-title class="title">
              Menu
            </v-list-item-title>
            <v-list-item-subtitle>
              What we have to offer
            </v-list-item-subtitle>
          </v-list-item-content>
        </v-list-item>

        <v-divider></v-divider>

        <v-list
          nav
        >
          <v-list-item
            v-for="item in items"
            :key="item.title"
            link
          >
            <v-list-item-icon>
              <v-icon>{{ item.icon }}</v-icon>
            </v-list-item-icon>

            <v-list-item-content>
              <v-list-item-title>{{ item.title }}</v-list-item-title>
            </v-list-item-content>
          </v-list-item>
        </v-list>
      </v-navigation-drawer>

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
  </div>
</template>

<script>
export default {
  name: 'TheNavigation',
  data () {
    return {
      drawer: false,
      items: [
        { title: 'Home', icon: 'mdi-home' },
        { title: 'Games', icon: 'mdi-dice-d20' },
        { title: 'Cafe', icon: 'mdi-food-fork-drink' },
        { title: 'Space', icon: 'mdi-table-chair' },
        { title: 'Community', icon: 'mdi-party-popper' },
        { title: 'Events', icon: 'mdi-calendar' },
        { title: 'Staff', icon: 'mdi-account-multiple' },
        { title: 'Contact', icon: 'mdi-help-circle' }
      ]
    }
  }
}
</script>

<style lang="css" scoped>
</style>
