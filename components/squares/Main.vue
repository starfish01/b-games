<template>
  <section>
    <div class="header">Timer:</div>
    <div class="box">
        <ViewOne :buttons="buttons"/>
    </div>
  </section>
</template>

<script>
import ViewOne from '~/components/squares/square-layout/ViewOne';
export default {
    components: {
        ViewOne
    },
    data () {
        return {
            buttons: [1,2,4,3]
        }
    }
}
</script>

<style lang="scss" scoped>
.box {
  background: red;
  width: 500px;
  height: 500px;
}
</style>
