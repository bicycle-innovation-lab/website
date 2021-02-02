<template>
  <nuxt-link
    to="/about"
    class="btn"
  >
    <svg width="13px" height="10px" viewBox="0 0 13 10">
      <path d="M1,5 L11,5" />
      <polyline points="8 1 12 5 8 9" />
    </svg>
    {{ text }}
  </nuxt-link>
</template>

<script>
export default {
  name: 'Btn',

  props: {
    text: {
      type: String,
      required: true
    },
    link: {
      type: String,
      required: true
    }
  }
}
</script>

<style lang="scss" scoped>
@import '../../assets/styles/abstracts/include-media';

.btn {
  --size: 1.5em;
  font-size: 1.3em;
  color: var(--text-color);
  padding-right: 2em;
  text-transform: uppercase;
  font-weight: bold;
  text-decoration: none;
  display: inline-flex;
  align-items: center;
  position: relative;
  z-index: 1;
  transition: color .1s ease-out;
}

.btn svg {
  stroke-width: 1;
  stroke: var(--black);
  fill: none;
  stroke-linecap: round;
  stroke-linejoin: round;
/*   background-color: var(--red); */
  width: var(--size);
  height: var(--size);
  margin-right: 1em;
  border-radius: 50%;
  padding: 1em;
  transform: rotate(45deg);
  transition: transform cubic-bezier(0.785, 0.135, 0.15, 0.86) 0.1s;

  @media (prefers-color-scheme: light) {
    stroke: var(--primary-color);
  }
}

.btn::before {
  content: "";
  height: calc(var(--size) + 2em);
  width: calc(var(--size) + 2em);
  border-radius: calc(45px + 3em);
  background-color: var(--primary-color);
  position: absolute;
  z-index: -1;
  transition: width cubic-bezier(0.785, 0.135, 0.15, 0.86) 0.15s;

  @media (prefers-color-scheme: light) {
    background-color: var(--black);
  }
}

.btn:hover {
  color: var(--black);

  @media (prefers-color-scheme: light) {
    color: var(--primary-color);
  }
}

.btn:hover svg {
  transform: rotate(0deg);
}

.btn:hover::before{
  width: 100%;
}
</style>
