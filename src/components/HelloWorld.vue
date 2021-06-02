<template>
  x-scroll
 <div class="x_scroll">
 <div class="scroll_child"></div>
 <div class="scroll_child"></div>
 <div class="scroll_child"></div>
 <div class="scroll_child"></div>
 <div class="scroll_child"></div>
 <div class="scroll_child"></div>
 </div>

  y-scroll
 <div class="y_scroll">
 <div class="scroll_child"></div>
 <div class="scroll_child"></div>
 <div class="scroll_child"></div>
 <div class="scroll_child"></div>
 <div class="scroll_child"></div>
 <div class="scroll_child"></div>
 </div>
 text-ellipsis
 <div class="text_ellipsis">
 <p>单行省略单行省略单行省略单行省略单行省略</p>
 <p>多行省略多行省略多行省略多行省略多行省略多行省略多行省略多行省略多行省略</p>
 </div>
</template>

<script>
export default {
  name: 'HelloWorld',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="less" scoped>
.x_scroll{
  width: 400px;
  height: 100px;
  display: -webkit-box;
  overflow-x: auto;
  margin: 0 auto; 
  div{
    width: 100px;
    height: 100px;
    background-color: #464464;
    margin-right: 10px;
  }
   &::-webkit-scrollbar {
    display: none;
  }
}
.y_scroll{
  width: 100px;
  height: 200px;
  overflow: hidden;
  overflow-y: scroll;
  margin: 0 auto; 
  div{
    width: 100px;
    height: 100px;
    background-color: #464464;
    margin-bottom: 10px;
  }
}
.text_ellipsis{
  margin: 0 auto;
  width: 200px;
  height: 200px;
  p:nth-child(1){
    overflow: hidden;
    text-overflow:ellipsis;
    white-space: nowrap;
  }
  p:nth-child(2){
    display: -webkit-box;
    -webkit-box-orient: vertical;
    -webkit-line-clamp: 2;
    overflow: hidden;
  }
}
</style>
