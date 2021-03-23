<template>
  <div id="app">
    <div id="nav">
      <router-link to="/"><IconLogo /></router-link>
      <NavigationItems />
    </div>
    <router-view/>
    <Footer />
  </div>
</template>

<script>
import IconLogo from '@/components/icons/IconLogo.vue'
import NavigationItems from '@/components/navigation-items.vue'
import Footer from '@/components/footer.vue'

export default {
  components: {
    IconLogo,
    NavigationItems,
    Footer
  }
}
</script>
<style lang="scss">
  #app {
  }
</style>
