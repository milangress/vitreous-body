<template>
  <h1 class="Logo">Point of <div class="block" style="width: 3em"></div><br> Vitreous Body</h1>
</template>
<style>
.Logo {
  animation: 1s appear;
  margin: auto;
}

.block {
  display: inline-block;
  height: 0.7em;
  min-width: 1em;
  background: white;
}

@keyframes appear {
  0% {
    opacity: 0;
  }
  100% {
    opacity: 1;
  }
}
</style>
