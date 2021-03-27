<template>
  <section>
    <div
      v-for="(button, key) in buttons"
      :key="key"
      @click="onButtonClick(button)"
      class="box box1"
    >
      {{ clicked.includes(button) ? button : '' }}
    </div>
  </section>
</template>

<script>
export default {
  props: ['buttons'],
  data() {
    return {
      clicked: [],
    }
  },
  methods: {
    onButtonClick(e) {
      this.clicked.push(e)
    },
  },
}
</script>

<style lang="scss" scoped>
.box {
  background: blue;
  width: 50px;
  height: 50px;
  color: white;
  cursor: pointer;
  &:hover {
    background: lightblue;
  }
}
.box1 {
  // margin: auto;
}
.box2 {
}
.box3 {
}
</style>
