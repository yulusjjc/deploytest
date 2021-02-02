<template>
  <el-container>
    <el-header>
      <index-header></index-header>
    </el-header>
    <el-main>
      <div class="container">
        <index-card></index-card>
      </div>
    </el-main>
  </el-container>
</template>

<script>
import IndexHeader from './components/Header'
import IndexCard from './components/Card'
export default {
  name: 'Index',
  components: {
    IndexHeader,
    IndexCard
  },
  data () {
    return {
      count: 0
    }
  },
  methods: {
    load () {
      this.count += 2
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="stylus" scoped>
  @import '~styles/varibles.styl'
  .el-container
    width:100%
    background: #f4f4f4
    min-height:100vh
  .el-header
    background: #fff
    box-shadow: 0 1px 2px 0 rgba(0,0,0,.05)
  .el-main
    margin-top:10px
  .container
    width:100%
    max-width:$maxWidth
    margin:0 auto
</style>
