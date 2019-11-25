<template>
  <div class="home">
    <TheCarousel />
    <OfferCards />
    <EventsCards />
    <PartyPanel />
  </div>
</template>

<script>
// @ is an alias to /src
import TheCarousel from '@/components/home/TheCarousel.vue'
import OfferCards from '@/components/home/OfferCards.vue'
import EventsCards from '@/components/home/EventsCards.vue'
import PartyPanel from '@/components/home/PartyPanel.vue'

export default {
  name: 'home',
  components: {
    TheCarousel,
    OfferCards,
    EventsCards,
    PartyPanel
  }
}
</script>
