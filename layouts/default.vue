<template>
  <div>
    <div :class="{baggroundColor: this.$route.name === 'index'}" >
      <Header />
    </div>
    <Nuxt />
    <Footer />
  </div>
</template>
