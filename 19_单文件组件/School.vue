<!--组件的结构（页面html模版）-->
<template>
    <div id="demo">
      <h2>学校名称：{{schoolName}}</h2>
      <h2>学校地址：{{schoolAddress}}</h2>
      <button @click="showShowName">点击显示学校名称</button>
    </div>
</template>

<!--组件的交互（js数据交互）-->
<script>
    export default {
      name:'school',
      data(){
        return{
          schoolName:'清华大学',
          schoolAddress:'北京'
        }
      },
      methods:{
        showShowName(){
          alert(this.schoolName)
        }
      }
    }
</script>

<!--组件的样式（css样式）-->
<style>
  #demo{
    background-color: aquamarine;
  }
</style>