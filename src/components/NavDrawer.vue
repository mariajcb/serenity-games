<template lang="html">
  <v-navigation-drawer
    color="grey darken-4"
    v-if="drawer"
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
</template>

<script>
export default {
  name: 'NavDrawer',
  props: ['drawer'],
  data () {
    return {
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
