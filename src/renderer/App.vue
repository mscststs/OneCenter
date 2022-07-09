<template>
  <div id="app">
    <oHeader></oHeader>
    <div class="content flex-auto flex">
      <TabView></TabView>
      <!-- 全局弹框 -->
      <oDialog></oDialog>
    </div>
  </div>
</template>

<script>
import oHeader from './components/Header/'
import oDialog from './components/Dialog/'
import TabView from './components/TabView'
export default {
  name: 'App',
  components: {
    oHeader,
    oDialog,
    TabView
  }
}
</script>

<style>
  /* CSS */
</style>

<style lang="less">
@import "assets/style/theme.less";

html, body {
  padding:0;
  margin:0;
  width:100%;
  height:100%;
  transition:all 0.25s;
  box-sizing:border-box;
  overflow: hidden;
  #app {
    width:100%;
    height:100%;
    display:flex;
    background-color:@bgColor;
    flex-direction: column;
  }
}
</style>
