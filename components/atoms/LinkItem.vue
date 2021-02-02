<template>
  <nuxt-link :to="to">
    <slot />
    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20" fill="currentColor" aria-hidden="true">
      <path
        stroke-width="2"
        stroke-linecap="round"
        stroke-linejoin="round"
        fill-rule="evenodd"
        d="M10.293 3.293a1 1 0 011.414 0l6 6a1 1 0 010 1.414l-6 6a1 1 0 01-1.414-1.414L14.586 11H3a1 1 0 110-2h11.586l-4.293-4.293a1 1 0 010-1.414z"
        clip-rule="evenodd"
      />
    </svg>
  </nuxt-link>
</template>

<script>
export default {
  name: 'Link',

  props: {
    to: {
      type: String,
      required: true
    }
  }
}
</script>

<style lang="scss" scoped>
  a {
    text-decoration-color: transparent;
    text-decoration-thickness: 1em;
    text-decoration: none;

    & svg {
      height: 1rem;
      margin-left: .5rem;
      opacity: 1;
      transform: translateX(-5px);
      transition: all 0.2s ease-out;
    }

    a:link {

    }

    &:visited {
      color: var(--gray-400);
    }

    &:hover {
      color: var(--primary-color);

      & svg {
        transform: translateX(0);
        opacity: 1;
      }
    }

    &:active {

    }
  }
</style>
