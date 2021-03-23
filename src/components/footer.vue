<template>
    <footer>
        <p>Blech</p>
        <nav>
            <NavigationItems />
        </nav>
    </footer>
</template>
<script>
import NavigationItems from '@/components/navigation-items.vue'

export default {
  name: 'Footer',
  components: {
    NavigationItems
  }
}
</script>
