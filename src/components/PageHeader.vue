<template>

    <div style="display: flex; flex-direction: row; position: relative;">

        <img src="@/assets/logo.png" />

        <!-- https://element-plus.org/zh-CN/component/menu -->
        <el-menu mode="horizontal" default-active="index" :ellipsis="ellipsis" router>
            <el-menu-item index="index" route="/">首页</el-menu-item>
            <el-menu-item index="check" route="/about">预约体检</el-menu-item>
            <el-menu-item index="generate" route="/about">生成食谱</el-menu-item>
            <el-menu-item index="methods">配餐方式</el-menu-item>
            <el-menu-item index="feedback">用户反馈</el-menu-item>
        </el-menu>

        <el-button type="primary" plain>注册</el-button>
        <el-button type="primary">登录</el-button>
    </div>
</template>

<style>
.el-menu {
    flex-grow: 1;
    position: absolute;
}

.el-menu-item {
    flex-grow: 1;
}
</style>

<script>
export default {
    data() {
        return {
            indexImages: [
                require("@/assets/logo.png"),
                require("@/assets/logo.png"),

            ],
            ellipsis: false
        }
    }
}
</script>