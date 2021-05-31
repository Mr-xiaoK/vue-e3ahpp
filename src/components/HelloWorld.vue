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
</template>

<script>
export default {
  name: 'HelloWorld',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="less" scoped>
.x_scroll{
  width: 500px;
  height: 100px;
  display: -webkit-box;
  overflow-x: auto;
  div{
    width: 100px;
    height: 100px;
    background-color: #464464;
    margin-right: 10px;
  }
}
</style>
