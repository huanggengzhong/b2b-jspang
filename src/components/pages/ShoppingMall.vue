<template>
    <div>
        {{msg}}
        <p>

            <van-button type="primary">主要按钮</van-button>
        </p>
        <van-row>
            <van-col span="8">span: 8</van-col>
            <van-col span="8">span: 8</van-col>
            <van-col span="8">span: 8</van-col>
        </van-row>
    </div>
</template>
<script>
export default {
    data() {
        return {
            msg: '这是首页',
        }
    },
}
</script>
<style>
</style>
