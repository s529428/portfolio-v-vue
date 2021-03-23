<template>
    <div class="hero-message">
        <svg class="canvas" viewBox="0 0 200 200">
            <h2 id="welcome-header" class="text">Hey there!</h2>
        </svg>
    </div>
</template>
<script>
export default {
  name: 'WelcomeMessage',
  methods: {

  },
  mounted () {
    const plugin = document.createElement('svg')
    plugin.setAttribute('src', 'https://cdn.skypack.dev/@svgdotjs/svg.js')
    plugin.async = true
    document.head.appendChild(plugin)
  }
}
</script>
<style>
.canvas {
    width: 75vmin;
    height: 75vmin;
    background: hsl(0, 0%, 100%);
}
</style>
