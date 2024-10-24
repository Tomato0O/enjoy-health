<template>
    <el-carousel>
        <el-carousel-item v-for="image in indexImages">
            <img :src="image" />
        </el-carousel-item>

    </el-carousel>
</template>

<style></style>

<script>
export default {
    data() {
        return {
            indexImages: [
                require("@/assets/logo.png"),
                require("@/assets/logo.png"),

            ]
        }
    }

}
</script>