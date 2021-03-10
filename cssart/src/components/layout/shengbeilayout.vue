<template>
  <div class="grail-layout">
    <div class="left">圣杯布局</div>
    <div class="right"></div>
    <div class="center">
      圣杯布局，父节点声明padding为左右列留出空位，将左右列固定在空位上
    </div>
  </div>
</template>

<script>
export default {
  name: "shengbeilayout",
};
</script>

<style lang="less" scoped>
.grail-layout {
  padding: 0 100px;
  width: 400px;
  height: 400px;
  margin: 0 auto;
}
.left {
  float: left;
  width: 100px;
  height: 100%;
  margin-left: -100px;
  background-color: #f66;
  writing-mode: vertical-rl;
  text-align: center;
  line-height: 100px;
  font-size: 28px;
}
.right {
  float: right;
  width: 100px;
  height: 100%;
  margin-right: -100px;
  background-color: #66f;
}
.center {
  height: 100%;
  background-color: #3c9;
}
</style>