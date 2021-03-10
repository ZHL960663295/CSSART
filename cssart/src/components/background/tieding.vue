<!-- 贴顶背景 -->
<template>
<div class="tieding">
    background
</div>
</template>

<script>
export default {
data() {
return {

}
},
//生命周期 - 创建完成（访问当前this实例）
created() {

},
//生命周期 - 挂载完成（访问DOM元素）
mounted() {

}
}
</script>
<style lang="less" scoped>
    .tieding{
        display: flex;
        justify-content: center;
        align-items: center;
        height: 300px;
        background: #000 url("../../assets/jinmuyan.jpg") no-repeat center top/auto 300px;
           text-shadow: 2px 2px 5px rgba(#000, .5);
           font-weight:bold ;
           color: #fff;
    }
</style>