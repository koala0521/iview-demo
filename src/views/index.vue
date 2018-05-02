<style scoped>
    .layout{
        border: 1px solid #d7dde4;
        background: #fff;
        position: relative;
        border-radius: 4px;
        overflow: hidden;
    }

    .layout-nav{
        width: 420px;
        margin: 0 auto;
        margin-right: 20px;
    }
    .layout-footer-center{
        text-align: center;
    }
    .ivu-layout{
        background: #fff;
    }
</style>
<template>
    <div class="layout">
        <Layout>
            <wHeader></wHeader>
            <Content :style="{margin: '88px 20px 0', minHeight: '500px'}">
                Content
            </Content>
            <Footer class="layout-footer-center">2011-2016 &copy; TalkingData</Footer>
        </Layout>
    </div>
</template>
<script>
    import wHeader from '../componets/header/index';
    export default {
        components:{
            wHeader
        }
    };
</script>