<template>
  <div class="hero">

    <div class="hero__bg" />

    <div class="grid">
      <div class="hero__text">
        <div>
          <p>
            Innovative <nuxt-link to="#">cykelforening</nuxt-link> hvor alle med interesse i cyklen kan hælpe med at udforske dens potentiale. Bliv medlem i dag og bliv en del af et <nuxt-link to="#">netværk</nuxt-link> med mange entusiaster. Få adgang til <nuxt-link to="#">vores værksted</nuxt-link>, lån cykler fra <nuxt-link to="#">cykelbiblioteket</nuxt-link>, deltag til <nuxt-link to="#">events</nuxt-link> og hjælp os med et af vores mange <nuxt-link to="#">andre projekter</nuxt-link>.
          </p>
          <nuxt-link
            to="/about"
            class="button button--primary"
          >
            Tilmeld mig
            <svg width="13px" height="10px" viewBox="0 0 13 10">
              <path d="M1,5 L11,5" />
              <polyline points="8 1 12 5 8 9" />
            </svg>
          </nuxt-link>
        </div>
      </div>
    </div>

  </div>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
.page-enter-active, .page-leave-active {
  .hero__bg {
    animation: grow-top cubic-bezier(0.785, 0.135, 0.15, 0.86) .5s forwards;
 }
}
.page-enter, .page-leave-active {

  .hero__bg {
    animation: grow-bottom cubic-bezier(0.785, 0.135, 0.15, 0.86) .3s both;
 }
}
</style>
