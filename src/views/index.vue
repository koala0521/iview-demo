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
    .banner-wrap{
        height: 300px;
        width: 100%;
        overflow: hidden;
    }
    .banner-wrap img{
        width: 100%;
        height: 100%;
    }

</style>
<template>
    <div class="layout">
        <Layout>
            <wHeader></wHeader>
            <Content :style="{margin: '64px 0', minHeight: '500px'}">
                <div class="banner-wrap" > 
                    <img src="../assets/img/bg.jpg" alt="">
                </div>
                <div :style="{ margin:'0  20px',minHeight:'1000px' }"> 啦啦啦啦 </div>
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