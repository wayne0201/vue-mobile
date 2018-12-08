<template>
  <div class="home">
    <div class="border-style">
      <span>{{text}}</span>
      <i class="seach-icon"></i>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: 'home',
  data() {
    return {
      text: '1px border'
    }
  }
}
</script>

<style scoped lang="stylus">
@import "~@/common/stylus/mixin.styl"
.home
  display flex
  flex-direction column
  justify-content center
  align-items center
.border-style
  display flex
  align-items center
  font-size 14px
  padding px2rem(10px)
  background #F9F9F9
  border-radius 4px
  border-1px(#CCCCCC, 4px)
  .seach-icon
    display inline-block
    margin-left 5px
    height 16px
    width 16px
    background-repeat no-repeat
    background-position center center
    background-size 16px 16px
    bg-image('~@/assets/search')
</style>
