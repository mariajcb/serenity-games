<template lang="html">
  <v-card
    class="mx-auto"
  >
    <v-container>
      <v-row dense>
        <v-col
          cols="12"
        >
          <v-card
            dark
            :color="item.color"
            flat
            class="py-7"
            v-for="item in items"
            :key="item.name"
          >
            <div class="d-flex flex-no-wrap justify-space-between">
              <v-avatar
                class="ma-3"
                size="125"
                circle
              >
                <v-img src="https://placekitten.com/125/125"></v-img>
              </v-avatar>
              <div>
                <v-card-title
                  class="headline mb-1 font-weight-black"
                >{{ item.name }}</v-card-title>
                <v-card-subtitle class="subtitle-1">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</v-card-subtitle>
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
  data () {
    return {
      items: [
        {
          name: 'Uncle Mike',
          src: require('@/assets/games.jpg'),
          color: '#85450A'
        },
        {
          name: 'Zac',
          src: require('@/assets/games.jpg'),
          color: 'outlined'
        },
        {
          name: 'Toro',
          src: require('@/assets/games.jpg'),
          color: 'deep-orange darken-4'
        },
        {
          name: 'Faith',
          src: require('@/assets/games.jpg'),
          color: 'black'
        },
        {
          name: 'Sam',
          src: require('@/assets/games.jpg'),
          color: '#85450A'
        },
        {
          name: 'Brent',
          src: require('@/assets/games.jpg'),
          color: 'outlined'
        }
      ]
    }
  }
}
</script>

<style lang="css" scoped>
</style>
