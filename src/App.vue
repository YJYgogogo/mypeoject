<template>
  <div class="container">
    <div class="header">头部</div>
    <div class="contant">内容区</div>
    <div class="footer">footer</div>
  </div>
</template>
<script>
export default {
  data () {
    return {

    }
  }
}
</script>
<style lang="scss">
html{
  font-size: 26.6666667vw;//设计稿以iphone6为基准 100/375 *100
}
body{
  font-size: 14px;
}
html,body,.container{
  width: 100%;
  height: 100%;
}
.container{
  display: flex;
  flex-direction: column;
  .header{
    height: 0.44rem;
    background: red;
  }
  .contant{
    flex: 1;
    overflow: auto;//产生滚动条
  }
  .footer{
    height: 0.44rem;
    background: grey;
  }
}
</style>
