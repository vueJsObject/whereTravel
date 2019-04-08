<template>
<div class="header">
    <div class="header-left">
        <div class="iconfont back-icon">&#xe624;</div>
    </div>
    <div class="header-input">
        <span class="iconfont">&#xe632;</span>
        输入城市/景点/游玩主题
    </div>
    <div class="header-right">
        <span class="iconfont">&#xe64a;</span>
        城市
    </div>
</div>
</template>
<script>
export default {
  name:'homeHeader'
}
</script>
<style lang="stylus" scoped>
// @import '~@/assets/styles/varibles.styl';
@import '~styles/varibles.styl';
.header
   display:flex
   line-height:.86rem
   background:$bgColor
   color:#fff
   .header-left
     width:0.64rem
     float: left
     .back-icon
       text-align:center
       font-size:.4rem
   .header-input 
     flex:1
     height:0.64rem
     line-height:0.64rem
     margin-top:.12rem
     margin-left:.2rem
     padding-left:.2rem
     background:#ffffff
     border-radius:.1rem
     color:#ccc
   .header-right
     width:1.24rem
     float:right
     text-align:center
</style>

