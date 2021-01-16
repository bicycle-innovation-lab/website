<template>
  <header class="grid header">
    <nav>
      <nuxt-link class="header__logo" to="/" :class="{notIndex: this.$route.name !== 'index'}">
        <svg width="13px" height="10px" viewBox="0 0 13 10">
          <path d="M1,5 L11,5" />
          <polyline points="8 1 12 5 8 9" />
        </svg>
        <h1>Bicycle Innovation Lab</h1>
      </nuxt-link>

      <div class="header__social">
        <social-icons />
      </div>
    </nav>
  </header>
</template>

<script>
import SocialIcons from './Social-icons.vue'

export default {
  components: { SocialIcons }
}
</script>

<style lang="scss" scoped>

</style>
