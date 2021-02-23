<template>
  <div class="home">
    <HomeSection />
  </div>
</template>

<script>
import HomeSection from '@/components/home-section.vue'

import { mapState } from 'vuex'

export default {
  name: 'Home-Section',
  components: {
    HomeSection
  },
  computed: {
    ...mapState([
      'work'
    ])
  }
}
</script>
