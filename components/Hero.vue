<template>
  <div class="bg">
    <div class="container">
      <Header />
      <div class="main">
        <div class="lead">
          <h2>
            Copenhagens most innovative bike aktivist
          </h2>
          <p>
            Forening med åben deltagelse, hvor alle med interesse i cyklen kan hælpe
            med at udforske cyklens potentiale. Bliv en del af et netværk med mange
            cykel aktivister.
          </p>
          <nuxt-link
            to="/about"
            class="button button--primary"
          >
            Become a member
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

.bg {
  background: var(--red-color) url("../static/images/hero-image-halftone.jpg") no-repeat 60% bottom;
  height: 80vh;
}

.main {
  display: flex;
  max-width: 50%;

  h2 {
    font-size: 5rem;
    line-height: 5rem;
  }

  picture {
    align-self: flex-end;
    img {
      width: 100%;
      object-fit: cover;
    }
  }
}

</style>
