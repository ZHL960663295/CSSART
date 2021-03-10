<!-- attr()属性函数 -->
<template>
<div>
    <h1 class="hello" data-name="玩转css的艺术之美"></h1>
    <a class="hover-tips btn-1" href="https://www.baidu.com" data-msg="Hello World">提示框</a>
    <a class="hover-tips btn-2" href="https://www.baidu.com"></a>
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
div{
    text-align: center;
}
a{
    display: block;
}
h1{
    &::before{
        content: attr(class);
    }
    &::after{
        content: attr(data-name);
    }
}
.hover-tips{
    position: relative;
    padding: 0 20px;
    border-radius: 10px;
    height: 40px;
    width: 160px;
    background-color: #66f;
    line-height: 40px;
    color: #fff;
    & + .hover-tips{
        margin-left: 10px;
    }
    &.btn-1{
        &::after{
            position: absolute;
            left: 0;
            top: 0;
            border-radius: 5px;
            width: 100%;
            height: 100%;
            background-color: rgba(222, 222, 222, .5);
            opacity: 0;
            text-align: center;
            font-size: 12px;
            content: attr(data-msg);
            transition: all 300ms;
        }
        &:hover::after{
            left:calc(100% + 20px);
            opacity: 1;
        }
    }
    &.btn-2:empty::after{
        content: attr(href)
    }
}
</style>