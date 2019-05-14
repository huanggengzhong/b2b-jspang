<template>
    <div>
        {{msg}}
        <p>

            <van-button type="primary">主要按钮</van-button>
        </p>
        <van-row>
            <van-col span="8">三个平分</van-col>
            <van-col span="8">三个平分</van-col>
            <van-col span="8">三个平分</van-col>
        </van-row>
        <van-row>
            <van-col span="4">四份</van-col>
            <van-col span="10" offset="4">十份,偏移了4份</van-col>
            <van-col span="6"></van-col>
        </van-row>

        <van-row>
            <van-col offset="12" span="12">offset: 12, span: 12</van-col>
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
