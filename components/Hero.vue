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
        <picture>
          <source>
          <source srcset="@/static/images/hero-image.avif" type="image/avif">
          <source srcset="@/static/images/hero-image.webp" type="image/webp">
          <img src="@/static/images/hero-image.png" alt="">
        </picture>
      </div>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>

.bg {
  background: var(#{--red-color});
  height: 80vh;
}

.main {
  display: flex;

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
