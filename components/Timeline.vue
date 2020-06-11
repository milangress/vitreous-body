<template>
  <svg id="Ebene_1" data-name="Ebene 1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 933 64.19" @mousemove="mousemove" >
    <defs>
      <style>
        .cls-1,.cls-3,.cls-4{fill:none;stroke:#fff;stroke-miterlimit:10;}
        .cls-1,.cls-3{stroke-width:2px;}
        .cls-2{fill:#fff;}
        .cls-3{stroke-linecap:round;}
      </style>
    </defs>
    <line class="cls-1" y1="54.68" x2="448.93" y2="54.68"/>
    <path class="cls-2" d="M461,64c-5.68,2.11-12.73,5.7-17.09,9.51L447.35,64l-3.44-9.51C448.27,58.3,455.32,61.89,461,64Z" transform="translate(0 -9.32)"/>
    <line class="cls-3" x1="471" y1="54.68" x2="932" y2="54.68"/>
    <g @style="left=mousemove">
    <line class="cls-4" x1="474.5" y1="14.18" x2="495.97" y2="14.57"/>
    <path class="cls-2" d="M502,24a30.27,30.27,0,0,0-8.63,4.6l1.8-4.72-1.63-4.79A30.2,30.2,0,0,0,502,24Z" transform="translate(0 -9.32)"/>
    <line class="cls-4" x1="434" y1="14.68" x2="412.53" y2="14.29"/>
    <path class="cls-2" d="M406.5,23.5a30.27,30.27,0,0,0,8.63-4.6l-1.8,4.72L415,28.41A30.2,30.2,0,0,0,406.5,23.5Z" transform="translate(0 -9.32)"/>
      <path class="cls-2" d="M452.38,30c0-2.57,1.09-4.58,3.53-6.64l1.43-1.22c2.52-2.14,3.36-3.74,3.36-5.46,0-2.52-2.23-4.07-5.25-4.07-4,0-6,2.56-6.35,5.67l-3.19-.93c.42-4.32,4-8,9.7-8a12.36,12.36,0,0,1,3.62.63,7,7,0,0,1,5,6.64c0,3.32-2.14,5.25-4.7,7.56l-1.34,1.22c-2,1.8-2.57,2.81-2.57,5.08v.46h-3.23Zm0,4.32h3.23v4.84h-3.23Z" transform="translate(0 -9.32)"/>
    </g>
  </svg>
</template>

<script>
    export default {
      name: "Timeline",
      data() {
          return {
            start: 0
          }
      },
      methods: {
        mousemove: function(e) {
          return e.clientX
          //console.log(e.clientX, e.clientY);
        }
      }

    }
</script>

<style scoped>

</style>
