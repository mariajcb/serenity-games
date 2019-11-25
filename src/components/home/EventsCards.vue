<template lang="html">
  <div class="pa-7">
    <h2 class="text-uppercase">Upcoming Events</h2>
    <v-row>
      <v-col cols="12">
        <v-row>
          <v-card
            max-width="350"
            class="mx-auto"
            outlined
            v-for="item in items"
            :key="item.date"
          >
            <v-list-item>
              <v-list-item-avatar tile size="50" class="ml-n4 mt-2 font-weight-bold" color="orange darken-3">{{item.date}}</v-list-item-avatar>
              <v-list-item-subtitle class="font-weight-medium orange--text text--darken-3">{{item.subtitle}}</v-list-item-subtitle>
            </v-list-item>

            <v-img
              src="@/assets/FNM.jpg"
              height="194"
            ></v-img>

            <v-list-item-title v-html="item.title" class="headline ml-4 mt-4 font-weight-bold">{{item.title}}</v-list-item-title>
            <v-card-actions>
              <v-btn
                text
                color="orange darken-3">
                RSVP
              </v-btn>
            </v-card-actions>
            <v-card-text class="font-weight-medium">
              {{item.text}}
            </v-card-text>
          </v-card>
        </v-row>
      </v-col>
    </v-row>
    <v-btn class="mt-8 font-weight-black" color="amber" light large>
      See More <v-icon>mdi-chevron-right</v-icon>
    </v-btn>
  </div>
</template>

<script>
export default {
  name: 'EventsCards',
  data () {
    return {
      items: [
        {
          date: 'Nov 29',
          title: 'Pioneer Friday Night Magic',
          subtitle: '8 PM Every Friday until Dec 27, 2019',
          img: '@/assets/FNM.jpg',
          text: 'Pioneer will utilize sets from Return to Ravnica forward. Bring your Modern deck or fledgling Pioneer deck, and we will hang out, trade, build, and play! Entry - $5 (monies returned in Store Credit with promo pack support).'
        },
        {
          date: 'Jan 4',
          title: 'Star Wars Legion <br> Prime Championship',
          subtitle: 'Saturday, 9 AM – 8 PM',
          img: '@/assets/sw-legion.jpg',
          text: 'This epic Legion competition will gather players from near and far for a day of high-energy competition, and the winner will earn an invitation to the Star Wars: Legion World Championship!'
        },
        {
          date: 'Nov 31',
          title: 'Modern Friday Night Magic',
          subtitle: '8 PM Every Friday until Apr 3, 2020',
          img: '@/assets/modern.jpg',
          text: 'Entry $5. Swiss - Recommended Rounds. FNM Promos and Store Credit payout'
        }
      ]
    }
  }
}
</script>

<style lang="css" scoped>
</style>
