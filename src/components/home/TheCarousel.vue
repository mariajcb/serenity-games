<template lang="html">
<v-carousel>
  <v-carousel-item
    v-for="(item, i) in items"
    :key="i"
    :src="item.src"
    reverse-transition="fade-transition"
    transition="fade-transition"
  >
    <v-sheet
      color="transparent"
      height="100%"
      tile
    >
      <v-row
        class="fill-height"
        align="center"
        justify="center"
      >
        <div class="display-3 font-weight-medium">{{ item.title }}</div>
      </v-row>
    </v-sheet>
  </v-carousel-item>
</v-carousel>
</template>

<script>
export default {
  data () {
    return {
      items: [
        {
          src: require('@/assets/games.jpg'),
          title: 'GAMES'
        },
        {
          src: require('@/assets/food.jpg'),
          title: 'FOOD'
        },
        {
          src: require('@/assets/community.jpg'),
          title: 'COMMUNITY'
        }
      ]
    }
  }
}
</script>
