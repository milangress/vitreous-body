<template lang="pug">
  .container
    .cover
      div
        logo
        .text_container
          p
            BlockBox(width=3)
            | 'Point of Vitreous Body' considers the total sum of sensory networks
            BlockBox(width=3 isHidden)
            | —cell phones, surveillance cameras, satellites, sensors— as computerized eyes.
            BlockBox(width=4)
            | Sensing fragments that gain power over the human physical and social body.
            BlockBox(width=2)
            | It looks at the point in time when more computerized eyes look at our world than human eyes.
            BlockBox(width=6)
      video(autoplay="autoplay" class="cover_video" loop="loop" muted="muted" playsinline="" src="/videos/cover-neu.mp4")
    h1.title
      | vitreous body
</template>

<script>
  import Logo from '~/components/Logo.vue'
  import BlockBox from '~/components/block-box.vue'

  export default {
    layout: 'default',
    components: {
      Logo,
      BlockBox,
    }
  }
</script>

<style>
  .cover {
    min-height: 100vh;
    padding: 2rem 4rem;

  }
  .text_container {
    max-width: 1000px;
    font-size: 1.6rem;
  }

  .links {
    padding-top: 15px;
  }
  .block {
    display: inline-block;
    height: 0.7em;
    min-width: 1em;
    background: white;
    margin: 0 0.1em;
  }

  .cover_video {
    position: absolute;
    left: 0;
    top: 0;
    z-index: -10;
    width: 100%;
    height: 100%;
    object-fit: cover;
  }
</style>
