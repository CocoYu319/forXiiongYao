<template>
  <div>
    <span @click="onClick">点击</span>
  </div>
</template>

<script>
import axios from 'axios'
export default {
  components: {
  },
  created () {},
  data () {
    return {}
  },
  methods: {
    onClick () {
      axios.get('k8s.1400720231.cn/api/index').then((res) => {
        console.log('数据：', res)
      })
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
