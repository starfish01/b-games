<template>
  <section class="section">
    <h2 class="title is-3">
      "Just start <b-icon icon="rocket" size="is-large" />"
    </h2>
    <h3 class="subtitle is-6 has-text-grey">
      Author: <a href="https://github.com/anteriovieira"> Antério Vieira </a>
    </h3>

    <Main />
  </section>
</template>
<script>
import Main from '~/components/squares/Main'

export default {
  components: {
    Main,
  },
}
</script>
<style lang="scss" scoped>
.box {
  background: red;
  width: 500px;
  height: 500px;
}
</style>
