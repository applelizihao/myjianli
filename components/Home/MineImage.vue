<template>
  <div class="row">
    <div class="col-md-12 col-lg-4 text-white text-center">
      <h3>前端工程师</h3>
      <front-end-engineer />
    </div>
    <div id="userimg" class="col-md-12 col-lg-4 text-center">
      <img src="@/static/img/mine.jpg" width="300" style="border-radius:50%">
    </div>
    <div class="col-md-12 col-lg-4 text-white text-center">
      <h3 class="mb-2">
        开发运维
      </h3>
      <dev-ops />
      <div class="mt-3">
        <h3>
          项目案例
        </h3>
        <ul class="list-unstyled d-flex justify-content-center flex-wrap">
          <li class="mx-2">
            <a target="_blank" href="https://www.wayon.com">威洋石材</a>
          </li>
          <li class="mx-2">
            <a target="_blank" href="https://www.rifeng.com/">日丰</a>
          </li>
          <li class="mx-2">
            <a target="_blank" href="https://applelizihao.github.io/driver/index.html">驾考一点通</a>
          </li>
          <li class="mx-2">
            <a target="_blank" href="http://119.29.200.195:888/user/login">博客CMS系统 <span class="text-danger" style="font-size:12px">(*开发中)</span></a>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>
<script>
import DevOps from './DevOps.vue'
import FrontEndEngineer from './FrontEndEngineer.vue'
export default {
  name: '',
  middleware: 'authenticated',
  components: {
    FrontEndEngineer,
    DevOps
  },
  data () {
    return {}
  },
  computed: {},
  watch: {},
  created () {},
  mounted () {},
  methods: {}
}

</script>
<style>
  @media screen and (max-width:1024px) {
    #userimg {
      margin: 30px 0;
    }
  }

  .svg-group svg {
    margin: 5px 5px;
  }

</style>
