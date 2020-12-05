<template>
  <div id="curriculum-list" class="css-1lffeal">
    <ul class="curriculum-list">
      <li class="curriculum-item curriculum-item--reverse">
        <h3>
          April 2019 - May 2019
        </h3>
        <h2>
          <a class="text-white text-decoration-none" target="_blank" href="https://applelizihao.github.io/driver/index.html">驾考一点通APP</a>
        </h2>
        <div>
          <p class="mb-0">
            利用VUE，根据驾考一点通的排版模仿出来，题型数据利用JSON文件保存到本地，答题系统内有错题本系统，答题错误时将保存到本地储存里面，内置有收藏提醒系统，答题错误时还能报出该提醒正确答案的因果描述。
          </p>
          <ul>
            <li>错题本系统</li>
            <li>收藏本系统</li>
            <li>数据以JSON形式存放,含有科一和科四题型</li>
          </ul>
          <p>这是我第一次写Vue做出来的项目,没有使用UI框架,题型是从驾考一点通爬取下来,通过这个项目让我学习到了数组处理的方法,例如:数组去重和剔除数组指定索引元素</p>
        </div><div class="tags">
          <i>Vue</i>
          <i>Html</i>
          <i>Css</i>
          <i>Javascript</i>
        </div>
      </li>
      <li class="curriculum-item">
        <h3>
          Dec 2019 - Feb 2020
        </h3>
        <h2>
          <a href="https://www.wayon.com" class="text-white text-decoration-none" target="_blank">广州市威洋石材官网</a>
        </h2>
        <div>
          <p class="mb-0">
            全站高级定制的企业型网站,官网主要以展示产品和公司简介为主要内容,能达到谷歌跑分评测标准九十分,拥有比较不错的seo优化排名。
          </p>
          <ul>
            <li>中国地图查看分公司插件</li>
            <li>瀑布流异步加载产品图</li>
            <li>用户询盘表单</li>
            <li>TawkTo留言插件</li>
            <li>多语言网站,支持四种国家语言</li>
          </ul>
          <p>
            通过这个项目对瀑布流和异步滚动加载有了认识,对SEO方面也有一定的了解和网站打开速度优化问题方面。
          </p>
        </div>
        <div class="tags">
          <i>PHP</i>
          <i>CodeIgniter3</i>
          <i>HTML</i>
          <i>JavaScript</i>
          <i>BootStrap</i>
        </div>
      </li>
      <li class="curriculum-item curriculum-item--reverse">
        <h3>
          Apr 2020 - June 2020
        </h3>
        <h2>
          <a href="https://www.rifeng.com" class="text-white text-decoration-none" target="_blank">日丰企业集团官网</a>
        </h2>
        <div>
          <p class="mb-0">
            全站高级定制的外贸型企业网站,官网主要以展示产品和公司简介为主要内容。能筛选产品,筛选下载内容,单独的功能定制性表单具有上传文件功能的表单。
          </p>
          <ul>
            <li>按条件筛选产品</li>
            <li>按条件筛选下载内容文件</li>
            <li>搜索关键词模块</li>
          </ul>
        </div><div class="tags">
          <i>HTML</i>
          <i>CSS</i>
          <i>Jquery</i>
          <i>JAVASCRIPT</i>
          <i>ES6</i>
          <i>BootStrap</i>
          <i>CodeIgniter3</i>
          <i>PHP</i>
        </div>
      </li>
      <li class="curriculum-item">
        <h3>
          Nov 2020 - Dec 2020
        </h3>
        <h2>
          <a href="http://119.29.200.195:888/user/login" class="text-white text-decoration-none" target="_blank">博客CMS系统</a>
        </h2>
        <div>
          <p class="mb-0">
            采用Python+nodeJs+nuxtJs开发的博客系统,拥有文件模块系统,能进行可视化新建文件删除文件,编辑代码等操作,内含有文章和文章分类系统
          </p>
          <ul>
            <li>文件模块系统</li>
            <li>详情模块</li>
            <li>登录注册模块</li>
          </ul>
          <p>目前处于开发状态,双人项目,前后端分离。</p>
        </div>
        <div class="tags">
          <i>CodeIgniter3</i>
          <i>HTML</i>
          <i>JavaScript</i>
          <i>BootStrap</i>
          <i>Python</i>
          <i>NuxtJs</i>
          <i>Css</i>
        </div>
      </li>
    </ul>
  </div>
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
  methods: {}

}
</script>
<style scoped>
#curriculum-list{
    color:white
}
/*! CSS Used from: Embedded */
.css-1lffeal{display:-webkit-box;display:-moz-box;display:-ms-flexbox;display:-webkit-flex;display:flex;flex-direction:column;align-items:center;-webkit-box-orient:vertical;-webkit-box-direction:normal;-webkit-flex-direction:column;-webkit-box-align:center;-webkit-align-items:center;}
/*! CSS Used from: Embedded */
.curriculum-list{border-left:6px solid #3ea191;padding:1rem 2rem;margin-left:2rem;max-width:600px;-webkit-transform:translate(48%);-ms-transform:translate(48%);transform:translate(48%);transition:all 1s;}
.curriculum-item{position:relative;padding-left:1rem;margin-bottom:3rem;list-style:none;}
.curriculum-item--reverse{-webkit-transform:scaleX(-1) translate(670px);-ms-transform:scaleX(-1) translate(670px);transform:scaleX(-1) translate(670px);}
.curriculum-item--reverse>div,.curriculum-item--reverse>h2,.curriculum-item--reverse>h3{-webkit-transform:scaleX(-1);-ms-transform:scaleX(-1);transform:scaleX(-1);}
.curriculum-item--reverse h2,.curriculum-item--reverse h3{text-align:right;}
.curriculum-item h3{font-size:1rem;padding:0;margin:0;color:#3ea191;font-style:italic;font-weight:200;}
.curriculum-item h2{padding:0;margin:.2rem 0;}
.curriculum-item ul{list-style-type:disc;}
.curriculum-item div{font-size:.9rem;margin:.5rem 0;word-break:break-word;line-height:1.3rem;}
.curriculum-item img{height:40px;}
.tags{display:-webkit-box;display:-ms-flexbox;display:flex;-webkit-box-orient:horizontal;-webkit-box-direction:normal;-ms-flex-direction:row;flex-direction:row;-ms-flex-wrap:wrap;flex-wrap:wrap;}
.tags i{font-size:.8rem;padding:0 .5rem;margin:.2rem;line-height:1.6rem;background-color:#3ea191;color:#fff;border-radius:5px;}
.curriculum-item:before{position:absolute;left:-35.2px;left:-2.2rem;top:19.2px;top:1.2rem;content:"";height:30px;width:30px;border-radius:30px;background-color:#43bda6;border:4px solid #3ea191;-webkit-transform:translate(-50%);-ms-transform:translate(-50%);transform:translate(-50%);}
@media (max-width:1365px){
.curriculum-item--reverse,.curriculum-item--reverse>div,.curriculum-item--reverse>h2,.curriculum-item--reverse>h3{-webkit-transform:none;-ms-transform:none;transform:none;}
.curriculum-item--reverse h2,.curriculum-item--reverse h3{text-align:left;}
.curriculum-list{border-left:6px solid #3ea191;padding:1rem 2rem;margin-left:2rem;max-width:600px;-webkit-transform:none;-ms-transform:none;transform:none;}
}
@media (min-width:1365px){
li.curriculum-item.curriculum-item--reverse{
    left: 4.35rem;
}
}
</style>
