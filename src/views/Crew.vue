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
                <v-img src="@/assets/bio-photo.jpg"></v-img>
              </v-avatar>
              <div>
                <v-card-title
                  class="headline mb-1 font-weight-black"
                >{{ item.name }}</v-card-title>
                <v-card-subtitle class="subtitle-1">Scratch at door to be let outside, get let out then scratch at door immmediately after to be let back in plays league of legends for bathe private parts with tongue then lick owner's face shake treat bag. So you're just gonna scroll by without saying meowdy? push your water glass on the floor yet dismember a mouse and then regurgitate part</v-card-subtitle>
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
