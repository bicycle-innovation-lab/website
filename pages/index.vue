<template>
  <div>
    <Hero />
    <Projects />
  </div>
</template>

<script>
export default {}
</script>

<style lang="scss">
/* Transitions using the page hook */
.page-enter-active, .page-leave-active {
  transition: all .2s;

  .hero__bg {
    opacity: 1;
    animation: grow-top cubic-bezier(0.785, 0.135, 0.15, 0.86) .5s forwards;
 }
}
.page-enter, .page-leave-active {
  opacity: 0;
  transform-origin: 50% 50%;

  .hero__bg {
    opacity: 1;
    animation: grow-bottom cubic-bezier(0.785, 0.135, 0.15, 0.86) .3s both;
 }
}
</style>
