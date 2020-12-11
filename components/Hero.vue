<template>
  <div class="baggroundColor">
    <div class="container">
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
            <svg width="13px" height="10px" viewBox="0 0 13 10">
              <path d="M1,5 L11,5" />
              <polyline points="8 1 12 5 8 9" />
            </svg>
            <!-- <svg
              xmlns='http://www.w3.org/2000/svg'
              width='12.083'
              height='12.239'>
              <g data-name='Group 29' fill='none' stroke='black' stroke-linecap='round' stroke-linejoin='round' stroke-width='2'> <path data-name='Path 2' d='M6.378 1.414l4.705 4.705-4.705 4.705'/> <path data-name='Line 2' d='M10.502 6.073H1'/> </g></svg> -->
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

.baggroundColor {
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
