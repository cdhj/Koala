<template>
  <div class="tit">
    <div class="titLeft"><div class="iconfont">&#xe610;</div></div>
    <div class="titSearch"><span class="iconfont">&#xe60d;</span>电动牙刷</div>
    <div class="titRight"><div class="iconfont">&#xe620;</div></div>
  </div>
</template>

<script>
export default {
  name: 'HomeTitle'
}
</script>

<style scoped lang="stylus">
  .tit
    line-height:.41rem
    font-size :.13rem
    color:#999999
    display:flex
    align-items center
    .titLeft
      width .45rem
      display:flex
      justify-content:center
      align-items:center
      font-size .26rem
      color:red
    .titSearch
      height:.28rem
      box-sizing:border-box
      flex:1
      line-height .2rem
      border-radius:1.5rem
      border:3px solid red
      .iconfont
        color:red
        padding-left:.1rem
        padding-right:.18rem
    .titRight
      width:.45rem
      display:flex
      justify-content:center
      align-items:center
      font-size .26rem
      color:red
</style>
