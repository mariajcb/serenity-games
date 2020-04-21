<template lang="html">
  <v-row no-gutters>
    <v-col
      v-for="item in items"
      :key="item.title"
    >
      <v-card
        class="pa-2"
        :color="item.color"
        height="300"
        tile
        outlined
      >
        <v-card-title class="title">
          {{item.title}}
        </v-card-title>
        <v-card-text class="body-1">
          {{item.text}}
        </v-card-text>
        <v-card-actions>
          <v-btn
            text
            outlined
            :to="item.url"
          >
            {{ item.button }}
          </v-btn>
        </v-card-actions>
      </v-card>
    </v-col>
  </v-row>
</template>

<script>
export default {
  name: 'OfferCards',
  data () {
    return {
      items: [
        {
          title: 'Games',
          text: `Serenity Games supports gaming in all its myriad of forms!  From RPG's, Tabletop Games, Board Games, Collectible Card Games, as well as the accessories to complement them!`,
          url: '',
          color: '#85450A',
          button: 'We have a bunch'
        },
        {
          title: 'Food',
          text: `As we travel across the 'Verse, gamers need fuel! The Serenity Games Cafe is fully equipped to satisfy with delicious Air-Fried consumables, frosty sweet treats, or energizing coffee beverages.`,
          url: '',
          color: 'outlined',
          button: `Don't play hangry`
        },
        // {
        //   title: 'Space',
        //   subtitle: 'Not the one with planets',
        //   text: 'Tired of having to clean your house, only for your boardgame-loving friends to mess it up? Take advantage of our already clean facilities.',
        //   url: '',
        //   color: 'outlined'
        // },
        {
          title: 'Community',
          subtitle: 'Can`t buy it on Amazon',
          text: `Without those who entrust us to provide a quality atmosphere to forge their games, dreams, and friendships... well I reckon we'd just be another empty ship in the harbor.  Everything we do is for you.`,
          url: '',
          color: 'deep-orange darken-4',
          button: 'Our most prized resource'
        }
      ]
    }
  }
}
</script>

<style lang="css" scoped>
</style>
