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
            | —cell phones, surveillance cameras, satellites, body sensors—
            | as computerized eyes.
            BlockBox(:width=4)
            | Sensing fragments that gain power over the human physical and social body.
            BlockBox(:width=2)
            | It looks at the point in time when more computerized eyes look at our world than human eyes.
            BlockBox(:width=6)
      video(autoplay="autoplay" class="cover_video" loop="loop" muted="muted" playsinline="" src="/videos/cover-neu.mp4")
      iframe(src="silence.mp3" allow="autoplay" id="audio" style="display: none")
      //audio(id="player" loop controls)
        source(src="vitriousbody_a_mg_mixdownHQ_final.mp3" type="audio/mp3")
    .section_container.grid
      .text_container
        h2.title
          | The vitreous body
        p
          | The vitreous body (vitreous body, "glassy", from the Latin vitreus, corresponding to vitr(um) glass + -eus -ous) is the clear gel that fills the space between the lens and the retina of the eyeball of humans and other vertebrates.
      img(src="img/eye.png" style="grid-column: 5")
    .section_container.video_wrapper
      .text_container
        h2.title
          | Transparencies
        p
          | The 'Point of Vitreous Body' places itself in a post-privacy world. As more and more computerized eyes look at the world like human eyes, it becomes a more relevant ability to hide from these gazes. I propose the thesis that one cannot defend oneself against the x-raying gaze (therefor becoming a "transparent citizen"), but should rather try to become a completely transparent body. The attempt to have more privacy is already hopeless. Therefore resistance should be overcome and absolute transparency should be strived for.
      video(autoplay="autoplay" class="full_video" loop="loop" muted="muted" playsinline="" src="/videos/Knoten2_VR.mp4.densepose.mp4")
    Timeline
    .section_container
      .text_container
        p The 'Point of Vitreous Body' could already be reality! Or it could still be some time of in the future and depends highly on the inclusion of smartphones as 'Computerized Eyes'. Although in London alone are 630,000 non movable cameras in public spaces installed. With its 9 million inhabitants this means we already have a saturation of 7 'Computerized Eyes' per 100 People.
    .section_container.grid
      img(src="img/gan.gif" style="grid-column: 1; width: 150%")
      .text_container(style="grid-column: 3 / 6")
        h2.title
          | "Computerized Eyes"
        p
          | "Computerized Eyes" as a term describe the continuous antromorphisation of cameras. In part defined through there additional image processing with the aim to build more abstract models of reality (like tracking body movement) but also with increased levels of autonomous decision making. Through these decisions a new level of power shifts directly "inside" the camera. The underlying power often stem from regular power structures and in fact only partly move to the camera. The rest stays with the code and there creator. Yet the cameras recognition system and power execution often happens inside unobservable "black boxes" so a tangible shift does occur.
    AudioDescription
</template>

<script>
  import Logo from '~/components/Logo.vue'
  import BlockBox from '~/components/block-box.vue'
  import BigEye from '~/components/big-eye.vue'
  import AudioDescription from "~/components/AudioDescription"
  import Timeline from "~/components/Timeline"

  export default {
    layout: 'default',
    components: {
      Logo, BlockBox, BigEye, AudioDescription, Timeline
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
  .fullwidth {
    grid-column: span 6;
  }
  .section_container {
    padding: 2rem 4rem;
  }
  .grid {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr 1fr 1fr;
  }
  .video_wrapper {
    position: relative;
    min-height: 100vh;
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
  .full_video {
    object-fit: cover;
    width: 100vw;
    height: 100vh;
    position: absolute;
    top: 0;
    left: 0;
    z-index: -10;
  }
</style>
