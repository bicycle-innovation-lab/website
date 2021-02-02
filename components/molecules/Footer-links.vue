<template>
  <ul>
    <li v-for="(link, key) in links" :key="key">
      <link-item :to="link.to">
        {{ link.content }}
      </link-item>
    </li>
  </ul>
</template>

<script >
import LinkItem from '../atoms/LinkItem.vue'

export default {
  name: 'FooterLinks',

  components: { LinkItem },

  props: {
    links: {
      type: Array,
      required: true
    }
  }
}
</script>
