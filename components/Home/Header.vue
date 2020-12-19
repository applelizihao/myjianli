<template>
  <header class="py-3 px-5 d-flex justify-content-between">
    <h1 class="text-white h4" @click="print">
      @李梓豪
    </h1>
    <ul class=" list-unstyled d-flex">
      <li id="weixin_li" class="text-white mx-2 position-relative">
        <a class="text-white h4">
          <i class="fa fa-weixin" />
          <img id="weixin" width="100" class="position-absolute" src="@/static/img/weixin.jpg">
        </a>
      </li>
      <li class="text-white mx-2">
        <a class="text-white h4" target="_blank" href="https://wpa.qq.com/msgrd?v=3&uin=2184724790&site=qq&menu=yes">
          <i class="fa fa-qq" />
        </a>
      </li>
      <svg viewBox="0 0 800 800" width="30" class="ml-2">
        <path fill="#de2910" d="M0 0h800v800H0z" />
        <path d="M314 163L130 297l70-217 71 217L86 163h228zm56-109l70 29-74 18 50-58-7 76-39-65zm92 70l53 55-75-13 69-34-36 67-11-75zm17 116l26 72-63-43 76-3-60 47 21-73zm-65 83l-3 76-42-64 71 27-73 20 47-59z" fill="#ffde00" />
      </svg>
    </ul>
  </header>
</template>
<script>
export default {
  name: '',
  components: {},
  data () {
    return {}
  },
  computed: {},
  watch: {},
  created () {},
  mounted () {},
  methods: {
    print () {
      document.getElementById('userimg').style.display = 'none'
      // 调用打印功能
      window.print()
      document.getElementById('userimg').style.display = 'block'
    }

  }
}
</script>
<style scoped>
 #weixin{
    transition: all .3s;
    display: none;
    z-index: 999;
    left: -30px;
    top: 40px;
  }
  #weixin_li:hover #weixin{
    display: block;
  }
</style>
