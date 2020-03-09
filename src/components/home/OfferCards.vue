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
        <v-card-subtitle class="subtitle-1">
          {{item.subtitle}}
        </v-card-subtitle>
        <v-card-text>
          {{item.text}}
        </v-card-text>
        <v-card-actions>
          <v-btn
            text
            :to="item.url"
          >
            Learn More
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
          subtitle: 'We have a bunch',
          text: 'Roleplaying games, collectible card games, board games, tabletop games, under the table games, mind games, the most dangerous games!',
          url: '',
          color: 'outlined'
        },
        {
          title: 'Food',
          subtitle: 'Don`t play hangry',
          text: 'Our cafe has the latest in gourmet grub. Stuff your face and play some games. Don`t forget to say `please` when you order',
          url: '',
          color: 'amber darken-3'
        },
        {
          title: 'Space',
          subtitle: 'Not the one with planets',
          text: 'Tired of having to clean your house, only for your boardgame-loving friends to mess it up? Take advantage of our already clean facilities.',
          url: '',
          color: 'outlined'
        },
        {
          title: 'Community',
          subtitle: 'Can`t buy it on Amazon',
          text: 'Whether you are a beginner or a competitive player, no matter how obscure your interests are, you can find friends around here',
          url: '',
          color: 'deep-orange darken-4'
        }
      ]
    }
  }
}
</script>

<style lang="css" scoped>
</style>
