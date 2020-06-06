<template>
    <div class="block" v-bind:style="{width: width + 'em'}" v-bind:class="{isHidden: isHidden}"></div>
</template>

<script>
    export default {
        name: "block-box",
        props: {
          width: Number,
          isHidden: Boolean,
        }
    }
</script>

<style scoped>
  .block {
    display: inline-block;
    height: 0.7em;
    min-width: 1em;
    background: white;
    margin: 0 0.15em;
  }
  .isHidden {
    background: transparent;
  }
</style>
