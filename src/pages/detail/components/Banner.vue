<template>
  <div>
    <div class="banner" @click="handleBannerClick">
      <img class="banner-img" src="//img1.qunarzz.com/sight/p0/1812/82/820670c947d2eb92a3.img.jpg_600x330_2bc29f9c.jpg" alt="">
      <div class="banner-info">
        <div class="banner-tittle">盈香生态园</div>
        <div class="banner-number">
          <span class="iconfont banner-icon">&#xe632;</span>
          39
        </div>
      </div>
    </div>
    <common-gallary
    :imgs="imgs"
    v-show="showGallary"
    @close="handleGallaryClose"
    >
    </common-gallary>
  </div>
</template>
<script>
import CommonGallary from 'common/gallary/Gallary'
export default {
  name: 'DetailBanner',
  data () {
    return {
      showGallary: false,
      imgs: ['http://img1.qunarzz.com/sight/p0/1812/a4/a472cbac7838b253a3.img.jpg_r_800x800_65baccec.jpg',
        'http://img1.qunarzz.com/sight/p0/1812/e4/e4075348eff276eaa3.img.jpg_r_800x800_c16b9beb.jpg']
    }
  },
  methods: {
    handleBannerClick () {
      this.showGallary = true
    },
    handleGallaryClose () {
      this.showGallary = false
    }
  },
  components: {
    CommonGallary
  }
}
</script>
<style lang="stylus" scoped>
  .banner
    position: relative
    overflow: hidden
    height: 0
    padding-bottom: 55%
    .banner-img
      width: 100%
    .banner-info
      display: flex
      position: absolute
      left: 0
      right: 0
      bottom: 0
      line-height: .6rem
      color: #fff
      background-image: linear-gradient(top, rgba(0, 0, 0, 0), rgba(0, 0, 0, 0.8))
      .banner-tittle
        flex: 1
        font-size: .32rem
        padding: 0 .2rem
      .banner-number
        height: .32rem
        line-height: .32rem
        margin-top: .14rem
        padding: 0 .4rem
        border-radius: .2rem
        background: rgba(0,0,0,.8)
        font-size: .24rem
        .banner-icon
          font-size: .24rem
</style>
