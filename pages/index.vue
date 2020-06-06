<template lang="pug">
  .container
    BigEye
    .cover
      div
        logo
        .text_container
          p
            BlockBox(:width=3)
            | 'Point of Vitreous Body' considers the total sum of sensory networks
            BlockBox(:width=3 isHidden)
            | —cell phones, surveillance cameras, satellites, sensors—
            | as computerized eyes.
            BlockBox(:width=4)
            | Sensing fragments that gain power over the human physical and social body.
            BlockBox(:width=2)
            | It looks at the point in time when more computerized eyes look at our world than human eyes.
            BlockBox(:width=6)
      video(autoplay="autoplay" class="cover_video" loop="loop" muted="muted" playsinline="" src="/videos/cover-neu.mp4")
      iframe(src="silence.mp3" allow="autoplay" id="audio" style="display: none")
      audio(id="player" loop controls)
        source(src="vitriousbody_a_mg_mixdownHQ_final.mp3" type="audio/mp3")
    .section_container.grid
      .text_container
        h2.title
          | The vitreous body
        p
          | The vitreous body (vitreous body, "glassy", from the Latin vitreus, corresponding to vitr(um) glass + -eus -ous) is the clear gel that fills the space between the lens and the retina of the eyeball of humans and other vertebrates.
      img(src="img/eye.png" style="grid-column: 5")
      .text_container
        h2.title
          | Transparencies
        p
          | The 'Point of Vitreous Body' places itself in a post-privacy world. As more and more computerized eyes look at the world like human eyes, it becomes a more relevant ability to hide from these gazes. I propose the thesis that one cannot defend oneself against the x-raying gaze (therefor becoming a "transparent citizen"), but should rather try to become a completely transparent body. The attempt to have more privacy is already hopeless. Therefore resistance should be overcome and absolute transparency should be strived for.
</template>

<script>
  import Logo from '~/components/Logo.vue'
  import BlockBox from '~/components/block-box.vue'
  import BigEye from '~/components/big-eye.vue'

  export default {
    layout: 'default',
    components: {
      Logo,
      BlockBox,
      BigEye
    }
  }
</script>

<style>
  .cover {
    min-height: 100vh;
    padding: 2rem 4rem;

  }
  .text_container {
    padding-bottom: 4rem;
    max-width: 1000px;
    font-size: 1.6rem;
    grid-column: span 3;
  }
  .section_container {
    padding: 2rem 4rem;
  }
  .grid {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr 1fr 1fr;
  }
  #player {
    margin-top: 2rem;
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
