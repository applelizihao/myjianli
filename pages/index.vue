<template>
  <div style="background:#012f56">
    <Header />
    <div class="container">
      <!--  eslint-disable-next-line vue/attribute-hyphenation -->
      <MineImage :listData="listData" />
      <!--  eslint-disable-next-line vue/attribute-hyphenation -->
      <curriculum-list :listData="listData" class="mt-3" />
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
    return {
      listData: [{
        title: '广州市威洋石材官网',
        description: '全站高级定制的企业型网站,官网主要以展示产品和公司简介为主要内容,能达到谷歌跑分评测标准九十分,拥有比较不错的seo优化排名。',
        link: 'https://www.wayon.com/',
        time: '2019.12 - 2020.2',
        advantage: ['中国地图查看分公司插件', '瀑布流异步加载产品图', '用户询盘表单', 'TawkTo留言插件', '多语言网站,支持四种国家语言'],
        summary: '通过这个项目对瀑布流和异步滚动加载有了认识,对SEO方面也有一定的了解和网站打开速度优化问题方面。',
        tags: ['PHP', 'CodeIgniter3', 'HTML', 'JavaScript', 'BootStrap', 'Jquery']
      },
      {
        title: '日丰企业集团官网',
        description: '全站高级定制的外贸型企业网站,官网主要以展示产品和公司简介为主要内容。能筛选产品,筛选下载内容,单独的功能定制性表单具有上传文件功能的表单。',
        link: 'https://www.rifeng.com/',
        time: '2020.5 - 2020.7',
        advantage: ['按条件筛选产品', '按条件筛选下载内容文件', '搜索关键词模块'],
        summary: '',
        tags: ['PHP', 'CodeIgniter3', 'HTML', 'JavaScript', 'BootStrap', 'Jquery']
      },
      {
        title: '深圳市斯迈尔机械公司官网',
        description: '全站高级定制型网站,官网主要以展示冷凝器,冷却器等产品和公司最新新闻为主要内容,有独立定制的询盘发送功能让客户有更好的询价数量提升,拥有筛选机制,运用物理知识和代码逻辑进行高精度匹配产品,拥有五国多语言站点。',
        link: 'https://www.newincoolingtower.com/',
        time: '2020.5 - 2020.7',
        advantage: ['定制询盘', '多语言站点', 'addthis社交平台分享', '华氏度物理计算筛选产品模块', '视频模块', '下载文件模块'],
        summary: '',
        tags: ['PHP', 'CodeIgniter3', 'HTML', 'JavaScript', 'BootStrap', 'Jquery']
      },
      {
        title: '柠檬树集装箱官网',
        description: '全站高级定制型网站,官网主要以展示集装箱产品,公司最新新闻为主要内容,有独立定制的询盘发送功能让客户有更好的询价数量提升。',
        link: 'https://www.lemontree-house.com/',
        time: '2019.9 - 2019.11',
        advantage: ['定制询盘', '多语言站点'],
        summary: '',
        tags: ['PHP', 'CodeIgniter3', 'HTML', 'JavaScript', 'BootStrap', 'Jquery']
      }, {
        title: '驾考一点通APP',
        description: '利用VUE,根据驾考一点通的排版模仿出来,题型数据利用JSON文件保存到本地,答题系统内有错题本系统,答题错误时将保存到本地储存里面,内置有收藏提醒系统,答题错误时还能报出该题型正确答案的因果关系',
        link: 'https://applelizihao.github.io/driver/index.html#/',
        time: '2019.4 - 2019.6',
        advantage: ['错题本模块', '收藏本模块', '数据以JSON形式存放,含有科一和科四题型', '实现限制答题', '考试模块', '练习题模块', '答错提示模块'],
        summary: '这是我第一次写Vue做出来的项目,没有使用UI框架,题型是从驾考一点通爬取下来,通过这个项目让我学习到了数组处理的方法,例如:数组去重和剔除数组指定索引元素',
        tags: ['Vue', 'Html', 'Css', 'Javascript']
      }, {
        title: '博客CMS系统',
        description: '采用Python+nodeJs+nuxtJs开发的博客系统,拥有文件模块模块,能进行可视化新建文件删除文件,编辑代码等操作,内含有文章和文章分类模块',
        link: 'http://www.datasview.com/user/login',
        time: '2020.11 - 2020.12',
        advantage: ['文件模块模块', '详情模块', '登录注册模块'],
        summary: '目前处于开发状态,双人项目,前后端分离。',
        tags: ['CodeIgniter3', 'HTML', 'JavaScript', 'BootStrap', 'Python', 'NuxtJs', 'Css', 'Vue']
      }
      ]
    }
  },
  computed: {},
  watch: {},
  created () {},
  mounted () {

  },
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
