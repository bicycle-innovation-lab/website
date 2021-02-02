<template>
  <nuxt-link :to="`/${link}`" class="card">
    <article>
      <div>
        <nuxt-image class="card__image" :placeholder="true" :src="img" />
      </div>
      <h3 class="card__title">
        {{ title }}
      </h3>
      <p class="card__text">
        {{ description }}
      </p>
      <!-- <link-item :to="`/${link}`" class="card__link">
        Læs mere
      </link-item> -->
    </article>
  </nuxt-link>
</template>

<script>
import LinkItem from '../atoms/LinkItem'

export default {
  name: 'Card',

  components: { LinkItem },

  props: {
    img: {
      type: String,
      required: false,
      default: 'htps://placekitten.com/200/300'
    },
    title: {
      type: String,
      required: false,
      default: ''
    },
    description: {
      type: String,
      required: false,
      default: ''
    },
    link: {
      type: String,
      required: false,
      default: '404'
    }
  }
}
</script>

<style lang="scss" scoped>
.card {
  text-decoration: none;
  width: clamp(40ch, 45%, 75ch);
  margin-bottom: 5rem;
  transition: all .2s ease-out;

  div {
    overflow: hidden;
  }

  &__image {
    padding-bottom: 3rem;
    transform: scale(1.12);
    transition: transform .1s;
  }

  &__title {
    margin-top: 3rem;
    margin-bottom: 2rem;
  }

  &__text {
    margin-bottom: 3rem;
  }

  &__link {
   text-decoration: inherit;
   color: var(--white);
   font-size: clamp(0.9rem, 0.7636363636rem + 0.6818181818vw, 1.2rem);
  }

  &:hover {
    // background: darkgray;

    .card__image {
      transform:scale(1.05)
    }
  }
}
</style>
