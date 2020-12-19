<template>
  <div id="curriculum-list" class="css-1lffeal">
    <ul class="curriculum-list">
      <template v-for="(item,index) in listData">
        <li :key="index" class="curriculum-item" :class="{'curriculum-item--reverse':index%2==0}">
          <time>
            Dec 2019 - Feb 2020
          </time>
          <h2>
            <a :href="item.link" class="text-white text-decoration-none" target="_blank">{{ item.title }}</a>
          </h2>
          <div>
            <p class="mb-0">
              {{ item.description }}
            </p>
            <ul>
              <template v-for="(tage,i) in item.advantage">
                <li :key="i">
                  {{ tage }}
                </li>
              </template>
            </ul>
            <p v-if="item.summary">
              {{ item.summary }}
            </p>
          </div>
          <div class="tags">
            <template v-for="(tag,i) in item.tags">
              <i :key="i">{{ tag }}</i>
            </template>
          </div>
        </li>
      </template>
    </ul>
  </div>
</template>
<script>
export default {
  name: '',
  components: {},
  props: {
    listData: {
      type: Array,
      default: null
    }
  },
  data () {
    return {

    }
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
.curriculum-item time{
  color:white !important;
  display: block;
}
/*! CSS Used from: Embedded */
.css-1lffeal{display:-webkit-box;display:-moz-box;display:-ms-flexbox;display:-webkit-flex;display:flex;flex-direction:column;align-items:center;-webkit-box-orient:vertical;-webkit-box-direction:normal;-webkit-flex-direction:column;-webkit-box-align:center;-webkit-align-items:center;}
/*! CSS Used from: Embedded */
.curriculum-list{border-left:6px solid #3ea191;padding:1rem 2rem;margin-left:2rem;max-width:600px;-webkit-transform:translate(48%);-ms-transform:translate(48%);transform:translate(48%);transition:all 1s;}
.curriculum-item{position:relative;padding-left:1rem;margin-bottom:3rem;list-style:none;}
.curriculum-item--reverse{-webkit-transform:scaleX(-1) translate(670px);-ms-transform:scaleX(-1) translate(670px);transform:scaleX(-1) translate(670px);}
.curriculum-item--reverse>div,.curriculum-item--reverse>h2,.curriculum-item--reverse>time{-webkit-transform:scaleX(-1);-ms-transform:scaleX(-1);transform:scaleX(-1);}
.curriculum-item--reverse h2,.curriculum-item--reverse time{text-align:right;}
.curriculum-item time{font-size:1rem;padding:0;margin:0;color:#3ea191;font-style:italic;font-weight:200;}
.curriculum-item h2{padding:0;margin:.2rem 0;}
.curriculum-item ul{list-style-type:disc;}
.curriculum-item div{font-size:.9rem;margin:.5rem 0;word-break:break-word;line-height:1.3rem;}
.curriculum-item img{height:40px;}
.tags{display:-webkit-box;display:-ms-flexbox;display:flex;-webkit-box-orient:horizontal;-webkit-box-direction:normal;-ms-flex-direction:row;flex-direction:row;-ms-flex-wrap:wrap;flex-wrap:wrap;}
.tags i{font-size:.8rem;padding:0 .5rem;margin:.2rem;line-height:1.6rem;background-color:#3ea191;color:#fff;border-radius:5px;}
.curriculum-item:before{position:absolute;left:-35.2px;left:-2.2rem;top:19.2px;top:1.2rem;content:"";height:30px;width:30px;border-radius:30px;background-color:#43bda6;border:4px solid #3ea191;-webkit-transform:translate(-50%);-ms-transform:translate(-50%);transform:translate(-50%);}
@media (max-width:1365px){
.curriculum-item--reverse,.curriculum-item--reverse>div,.curriculum-item--reverse>h2,.curriculum-item--reverse>time{-webkit-transform:none;-ms-transform:none;transform:none;}
.curriculum-item--reverse h2,.curriculum-item--reverse time{text-align:left;}
.curriculum-list{border-left:6px solid #3ea191;padding:1rem 2rem;margin-left:2rem;max-width:600px;-webkit-transform:none;-ms-transform:none;transform:none;}
}
@media (min-width:1365px){
li.curriculum-item.curriculum-item--reverse{
    left: 4.35rem;
}
}
</style>
