<template>
  <div class="swiper">
    <div class="swiper-container">
      <div class="swiper-wrapper">
        <div class="swiper-slide" v-for="i of swiperList" :key="i.id">
          <img
            class="swiperImg"
            :src="i.imgUrl"
          >
        </div>
      </div>
      <div class="swiper-pagination"></div>
    </div>
  </div>
</template>

<script>
import Swiper from '../../../bower_components/swiper/dist/js/swiper'
import '../../../bower_components/swiper/dist/css/swiper.css'
export default {
  name: 'HomeSwiper',
  data () {
    return{
      swiperList:[
        {
          id:"0001",
          imgUrl:"https://haitao.nosdn1.127.net/f7df404c-1a68-4158-8b88-63202f8bcfa0T1901071745_960_480.jpg"
        },
        {
          id:"0002",
          imgUrl:"https://haitao.nosdn1.127.net/018a9c28-376a-47c6-b5b4-2930c94a8cb2T19010102103_960_480.jpg?imageView&thumbnail=750x0&quality=95&type=webp"
        },
        {
          id:"0003",
          imgUrl:"https://haitao.nos.netease.com/3dd929be-871f-4656-903d-c39c22ddadc5T19010102228_960_480.jpg?imageView&thumbnail=750x0&quality=95&type=webp"
        }
      ]
    }
  },
  mounted () {
    var mySwiper = new Swiper ('.swiper-container', {
      loop: true, // 循环模式选项
      pagination: {
        el: '.swiper-pagination',
        type:'fraction'
      },
      autoplay:true
    })
  }
}
</script>

<style scoped  lang="stylus">
  .swiper >>> .swiper-pagination-fraction
    font-size:12px !important
    text-align:left !important
    color: white !important
    margin-bottom:10px !important
    margin-left:10px !important
  .swiperImg
    width:100%
</style>
