<template>
  <div class="gl-page">
    <gl-nav-bar title="title"></gl-nav-bar>
    <button @click="hi">Click me</button>

    <gl-scroller class="scroller">
      <ul>
        <p :key="i" v-for="i in 100">{{i}}</p>
      </ul>
    </gl-scroller>
  </div>
</template>

<script>
export default {
  name: 'page-index',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  },

  methods: {
    hi () {
      alert('Hi you!')
    }
  }
}
</script>

<style lang="scss">
.scroller{
  width: 6rem;
  height: 6rem;
  margin: 10px auto;
  padding: 10px;
  background-color: #f4f4f4;
}
button{
  // border: 1px solid #333;
}
</style>
