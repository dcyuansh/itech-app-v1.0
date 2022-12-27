<template>
    <el-container>
      <el-header style="padding: 0px;">
        <!-- 导航栏 -->
        <v-header></v-header>
      </el-header>

      <el-main>
        <!-- 渲染组件 -->
        <router-view></router-view>
      </el-main>

       <!-- 页脚 -->
        <el-footer style="padding: 0px;">
          <v-footer></v-footer>
        </el-footer>
     
    </el-container>
</template>
  

<script>
import Header from '../components/Header.vue'
import Footer from '../components/Footer.vue'

export default {
  name: 'MenuIndex',
  data () {
    return {
    }
  },


  components: {
    'v-header': Header,
    'v-footer': Footer,
  }

}
</script>




<style scoped>
html,
body {
  /*设置内部填充为0，几个布局元素之间没有间距*/
  padding: 0px; 
  /*外部间距也是如此设置*/
  margin: 0px; 
  /*统一设置高度为100%*/
  height: 100%; 
}
</style>
