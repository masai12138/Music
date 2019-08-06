<template>
  <div id="app">
    <div class="header"><span class="header-title">{{title}}</span></div>
    <router-view/>
  </div>
</template>

<style>
.app{
  width: 100%;
  height: 100%;
  margin: 0;
  background-color:black;
}
.header{
  width: 100%;
  height: 64px;
  background-color: red;
  font-size: 20px;
  color: aliceblue;
  text-align: center;
  display: flex;
  flex-direction: column;
  justify-content: center;
  
}
</style>
<script>


export default {
  data : function(){
    return {
      title : '热门音乐排行榜'
    }
  }
}
</script>