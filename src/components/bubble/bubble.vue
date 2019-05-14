<template>
  <span class="bubble">
    {{ num }}
  </span>
</template>

<script>
  export default {
    name: 'bubble',
    props: {
      num: {
        type: Number
      }
    }
  }
</script>

<style lang="stylus" scoped>
  @import "~common/stylus/variable"

  .bubble
    display: inline-block
    padding: 0 5px
    height: 15px
    line-height: 18px
    text-align: center
    border-radius: 15px
    font-family: Helvetica
    font-weight: 700
    font-size: $fontsize-small-s
    color: $color-white
    background: linear-gradient(to right, $color-orange, $color-red)
</style>
