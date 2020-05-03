<template>
  <a
    :class="classList"
    class="no-underline hover:no-underline font-bold text-2xl lg:text-4xl"
    href="#"
  >METRIC DISPLAY</a>
</template>

<script>
export default {
  name: 'Logo',
  props: {
    isStickable: {
      type: Boolean,
      default: false
    },
    isSticky: {
      type: Boolean,
      default: false
    }
  },
  computed: {
    classList() {
      let classList = ''
      if (this.isStickable) {
        classList = this.isSticky ? 'logo-color' : 'text-white'
      } else {
        classList = 'logo-color'
      }
      return classList
    }
  }
}
</script>
<style>
.logo-color {
  color: #1565c0; /* Colors.blue[800] */
}
</style>