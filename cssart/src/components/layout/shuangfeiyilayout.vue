<!-- 双飞翼布局 -->
<template>
  <div class="grail-layout">
      <div class="left">
        双飞翼布局
      </div>
      <div class="right"></div>
      <div class="center">
        <div>
          双飞翼布局，中间列插入子节点并声明margin为左右列让出空位，将左右列固定在空位上
        </div>
      </div>
  </div>
</template>

<script>
export default {
  data() {
    return {};
  },
  //生命周期 - 创建完成（访问当前this实例）
  created() {},
  //生命周期 - 挂载完成（访问DOM元素）
  mounted() {},
};
</script>
<style lang="less" scoped>
  .grail-layout{
    width: 400px;
    height: 400px;
    margin: 0 auto;
    .left{
      float: left;
      width: 100px;
      height: 100%;
      background-color: #f66;
      writing-mode: vertical-lr;
      text-align: center;
      line-height: 100px;
      font-size: 28px;
    }
    .right{
      float: right;
      width: 100px;
      height: 100%;
      background-color: #66f;
    }
    .center{
      margin: 0 100px;
      height: 100%;
      background-color: #3c9;
    }
  }
</style>