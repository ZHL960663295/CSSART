<!-- 文本环绕 -->
<template>
  <div class="text-wrapping">
    <img src="../../assets/la.jpg" alt="" />
    XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
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
.text-wrapping {
      overflow: hidden;
    width: 400px;
    height: 300px;
    font-size: 20px;
    color: #f66;
    word-break: break-all;
  margin: 0 auto;
  img{
       float: left;
        margin: 10px;
        height: 200px;
  }
}
</style>