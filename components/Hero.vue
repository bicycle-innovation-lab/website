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

  .container {
    display: flex;
    flex-direction: column;
    height: 100%;
  }
}

.main {
  h2,
  p,
  a {
    opacity: 0;
    animation: fade-in-top ease .4s forwards;
  }
}

.main {
  display: flex;
  max-width: 500px;
  flex: 1;
  align-items: center;

  h2 {
    font-size: 2.8rem;
    line-height: 2.7rem;
    animation-delay: .2s;
  }

  p {
    font-size: 1.6rem;
    line-height: 1.8rem;
    animation-delay: .3s;
  }

  a{
    animation-delay: .4s;
  }
}

</style>
