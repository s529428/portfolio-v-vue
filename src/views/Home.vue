<template>
  <div class="home">
    <WelcomeMessage />
    <HomeSection />
  </div>
</template>

<script>
import HomeSection from '@/components/home-section.vue'
import WelcomeMessage from '@/components/welcome-message.vue'

import { mapState } from 'vuex'

export default {
  name: 'Home-Section',
  components: {
    HomeSection,
    WelcomeMessage
  },
  computed: {
    ...mapState([
      'work'
    ])
  }
}
</script>
