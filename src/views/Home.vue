<template>
  <div class="home">
    <TheCarousel />
    <OfferCards />
  </div>
</template>

<script>
// @ is an alias to /src
import TheCarousel from '@/components/home/TheCarousel.vue'
import OfferCards from '@/components/home/OfferCards.vue'

export default {
  name: 'home',
  components: {
    TheCarousel,
    OfferCards
  }
}
</script>
