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
          <template v-for="(item,index) in listData">
            <li :key="index" class="mx-2 project-title">
              <a target="_blank" :href="item.link" style="font-size:14px">{{ item.title }}</a>
            </li>
          </template>
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
              多谷网络科技有限公司 2019.5 - 2020.7
            </p>
            <p style="font-size: 13px">
              在该公司负责前后端cms建站开发，利用基于ci框架进行建站，一年制作完成的项目一百余个，基本日常工作跟客服沟通，跟业务了解需求，还原美工设计图，了解后进行数据绑定和功能实现。
            </p>
          </li>
          <li>
            <p class="m-0">
              涌现科技 2020.8 - 2020.12
            </p>
            <p style="font-size: 13px">
              主导一个github站点前端的制作,用vuejs+bootstrap技术编写,运用vuex全家桶,nuxtJs技术,参与git分支图（Graph）实现,完成下拉滚动无缝加载commit,并将这些commit进行绑定支付功能,调用第三方Strip国际支付完成功能,实现订单支付流程,订单交易流水图标。完成Wiki,Issue提问,回复,模块功能实现,。实现merge合并创建根据后端返回的数据进行前端页面展示与功能实现,类似GitlabMerge页面合并功能。利用nuxtjs
              ssr渲染进行project页面进行seo优化，利用docker打包成镜像交付给后端进行自动化部署。
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
  props: {
    listData: {
      type: Array,
      default: null
    }
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
.project-title a{
  color:white
}
.project-title a:hover{
  color: rgb(36, 104, 230);
}
.svg-group svg {
  margin: 5px 5px;
}
</style>
