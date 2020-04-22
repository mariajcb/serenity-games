<template>
  <div class="home">
    <TheCarousel />
    <OfferCards />
    <CoronaVirus />
    <!-- <PartyPanel /> -->
    <BioCard />
  </div>
</template>

<script>
// @ is an alias to /src
import TheCarousel from '@/components/home/TheCarousel.vue'
import OfferCards from '@/components/home/OfferCards.vue'
import CoronaVirus from '@/components/home/CoronaVirus.vue'
// import PartyPanel from '@/components/home/PartyPanel.vue'
import BioCard from '@/components/global/BioCard.vue'

export default {
  name: 'home',
  components: {
    TheCarousel,
    OfferCards,
    CoronaVirus,
    // PartyPanel,
    BioCard
  }
}
</script>
