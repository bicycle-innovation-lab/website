<template>
  <header class="container">
    <nuxt-link to="/" class="logo" :class="{notIndex: this.$route.name !== 'index'}">
      <svg width="13px" height="10px" viewBox="0 0 13 10">
        <path d="M1,5 L11,5" />
        <polyline points="8 1 12 5 8 9" />
      </svg>
      <h1>Bicycle Innovation Lab</h1>
    </nuxt-link>
    <div class="social">
      <a
        href="#"
      ><svg
        xmlns="http://www.w3.org/2000/svg"
        width="22.93"
        height="22.793"
        viewBox="0 0 22.93 22.793"
      >
        <path
          id="logo-facebook"
          d="M54.93,44.815A11.465,11.465,0,1,0,41.674,56.142V48.13H38.762V44.815h2.912V42.289c0-2.873,1.712-4.461,4.331-4.461a17.618,17.618,0,0,1,2.567.224v2.822H47.125a1.658,1.658,0,0,0-1.869,1.791v2.151h3.18l-.508,3.315H45.256v8.012A11.468,11.468,0,0,0,54.93,44.815Z"
          transform="translate(-32 -33.35)"
          fill="#010101"
          fill-rule="evenodd"
        />
      </svg>
      </a>
      <a
        href="#"
      ><svg
        xmlns="http://www.w3.org/2000/svg"
        width="23.042"
        height="23.042"
        viewBox="0 0 23.042 23.042"
      >
        <g id="logo-instagram" transform="translate(-32 -32)">
          <path
            id="Path_6"
            data-name="Path 6"
            d="M48.321,33.92a4.815,4.815,0,0,1,4.8,4.8v9.6a4.815,4.815,0,0,1-4.8,4.8h-9.6a4.815,4.815,0,0,1-4.8-4.8v-9.6a4.815,4.815,0,0,1,4.8-4.8h9.6m0-1.92h-9.6A6.74,6.74,0,0,0,32,38.721v9.6a6.74,6.74,0,0,0,6.721,6.721h9.6a6.74,6.74,0,0,0,6.721-6.721v-9.6A6.74,6.74,0,0,0,48.321,32Z"
            fill="#313131"
          />
          <path
            id="Path_7"
            data-name="Path 7"
            d="M350.847,109.7a1.514,1.514,0,1,1,1.074-.443A1.517,1.517,0,0,1,350.847,109.7Z"
            transform="translate(-301.134 -70.859)"
            fill="#313131"
          />
          <path
            id="Path_8"
            data-name="Path 8"
            d="M151.038,146.346a4.692,4.692,0,1,1-4.692,4.692,4.692,4.692,0,0,1,4.692-4.692m0-2.346a7.038,7.038,0,1,0,7.038,7.038A7.038,7.038,0,0,0,151.038,144Z"
            transform="translate(-107.517 -107.517)"
            fill="#313131"
          />
        </g>
      </svg>
      </a>
    </div>
  </header>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
header {
  position: relative;
  z-index: 1;
}

h1,
.social {
  opacity: 0;
  animation: fade-in-right ease .4s forwards;
}
header {
  display: flex;
  justify-content: space-between;
  align-items: baseline;
  padding-top: 3rem;
  // padding-bottom: 3rem;
  h1 {
    margin: 0;
    font-size: 1rem;
    text-transform: uppercase;
    letter-spacing: -0.016em;
    word-spacing: 0.08em;
  }

  .social {
    animation-delay: .3s;
    svg {
      width: 2rem;
    }
  }
}

.logo {
  display: inline-block;
  padding: 1.5rem 1.5rem 1.5rem 0;

  svg {
    transform: rotate(.5turn) translateX(-10px);
    opacity: 0;
    position: relative;
    bottom: 2px;
    margin-right: .7rem;
    fill: none;
    stroke-linecap: round;
    stroke-linejoin: round;
    stroke: var(--black);
    stroke-width: 2;
    transition: all 0.15s ease-out;
  }

  h1 {
    margin-left: -27px;
    display: inline-block;
    transition: all 0.15s ease-out;
    
  }
}

.logo.notIndex {
  svg {
    transform: rotate(.5turn) translateX(-2px);
    opacity: 1;
  }
  h1 {
    margin-left: -8px;
  }

  &:hover {
      svg {
      transform: rotate(.5turn) translateX(2px);
    }
  }
}

</style>
