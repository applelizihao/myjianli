<template>
  <div class="row">
    <div class="col-md-12 col-lg-4 text-white text-center">
      <h3>前端工程师</h3>
      <p>
        拥有两年前端工作经验,具备CMS开发经验,能独立完成建站项目并部署到服务器上,擅长用宝塔进行部署。熟悉并有实际经验优化vue
        seo优化并能搭建项目放到服务器运行。
      </p>
      <ul class="p-0">
        <li class="list-unstyled">
          常用UI框架:Bootstrap-Vue Vuetify
        </li>
      </ul>
      <front-end-engineer />
    </div>
    <div id="userimg" class="col-md-12 col-lg-4 text-center">
      <img
        src="@/static/img/mine.png"
        style="border-radius: 50%; width: 300px; height: 300px"
      >
    </div>
    <div class="col-md-12 col-lg-4 text-white text-center">
      <h3 class="mb-2">
        开发运维
      </h3>
      <dev-ops />
      <div class="mt-3">
        <h3>项目案例</h3>
        <ul class="list-unstyled d-flex justify-content-center flex-wrap">
          <li class="mx-2">
            <a target="_blank" href="https://www.wayon.com">威洋石材</a>
          </li>
          <li class="mx-2">
            <a target="_blank" href="https://www.rifeng.com/">日丰</a>
          </li>
          <li class="mx-2">
            <a
              target="_blank"
              href="https://applelizihao.github.io/driver/index.html"
            >驾考一点通</a>
          </li>
          <li class="mx-2">
            <a
              target="_blank"
              href="http://www.datasview.com/user/login"
            >博客CMS系统
            </a>
          </li>
        </ul>
      </div>
    </div>
    <div class="col-md-12 text-white">
      <div class="mt-3">
        <h3 class="mb-2">
          工作经历
        </h3>
        <ul class="list-unstyled d-flex flex-wrap p-0">
          <li>
            <p class="m-0">
              多谷网络科技有限公司 May 2019 - July 2020
            </p>
            <p style="font-size: 13px">
              在该公司负责前后端cms建站开发，利用基于ci框架进行建站，一年制作完成的项目一百余个，基本日常工作跟客服沟通，跟业务了解需求，还原美工设计图，了解后进行数据绑定和功能实现。
            </p>
          </li>
          <li>
            <p class="m-0">
              涌现科技 Aug 2020 - Dec 2020
            </p>
            <p style="font-size: 13px">
              类似做github项目 用vuejs+bootstrap技术写
              参与git分支图逻辑参与与实现，merge合并创建根据后端返回的数据进行前端页面展示。利用nuxtjs
              ssr渲染进行project页面进行seo优化，利用docker打包成镜像交付给后端进行自动化部署
            </p>
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
@media screen and (max-width: 1024px) {
  #userimg {
    margin: 30px 0;
  }
}

.svg-group svg {
  margin: 5px 5px;
}
</style>
