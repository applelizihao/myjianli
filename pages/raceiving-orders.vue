<template>
  <div>
    <!-- {{ description_raceiving_orders }} -->
  </div>
</template>

<script>
export default {
  name: '',
  components: {
    // [Button.name]: Button // 此处是引入组件名字的方法
  },
  data () {
    return {
      description_raceiving_orders: [{
        title: '网页PC端 移动端'
      }, {
        title: '响应式Web切图'
      }, {
        title: 'Vue切图页面 制作逻辑功能'
      }, {
        title: '独立站点建设（包后台）'
      }, {
        title: '仿站建站'
      }, {
        title: '定制Jquery效果 SVG效果'
      }, {
        title: '小程序制作 公众号制作'
      }]
    }
  },
  created () {

  },
  mounted () {

  },
  methods: {

  },
  head () {
    return {
      title: '前端技术外包服务',
      meta: [
        { hid: 'description', name: 'description', content: '前端技术外包服务' }
      ]
    }
  }
}
</script>

<style scoped lang="scss">

</style>
