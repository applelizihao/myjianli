<template>
  <div>
    <Header />
    <div class="container">
      <MineImage />
      <curriculum-list class="mt-3" />
    </div>
    <Footer class="mt-5" />
  </div>
</template>
<script>
import Header from '@/components/Home/Header'
import Footer from '@/components/Home/Footer'
import MineImage from '@/components/Home/MineImage'
import CurriculumList from '../components/Home/CurriculumList.vue'
export default {
  name: '',
  components: { Header, Footer, MineImage, CurriculumList },
  data () {
    return {}
  },
  computed: {},
  watch: {},
  created () {},
  mounted () {},
  methods: {},
  head () {
    return {
      title: '@LeeSinHao',
      meta: [
        { hid: 'description', name: 'description', content: '@LeeSinHao' }
      ]
    }
  }
}
</script>
<style lang='scss' scoped>
</style>
