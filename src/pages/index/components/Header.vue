<template>
  <div class="container header">
    <i class="logo el-icon-s-opportunity"></i>
    <div>
      <el-button type="primary" size="medium">按钮</el-button>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Header'
}
</script>

<style lang="stylus" scoped>
  @import '~styles/varibles.styl'
  @import "~styles/mixins.styl"
  .container
    width:100%
    max-width:$maxWidth
    margin:0 auto
  .header
    height:60px
    flexBetweenCenter()
    .logo
      font-size:30px
      color: $bgColor
</style>
