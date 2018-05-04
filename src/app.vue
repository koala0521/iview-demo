<style scoped >
    .layout{
        border: 1px solid #d7dde4;
        background: #fff;
        position: relative;
        border-radius: 4px;
        overflow: hidden;
    }
    .cont-width{
        width: 1200px;
        min-width: 1200px;
        margin: 0 auto;
    }
    .ivu-layout{
        background: #fff;
    }
</style>

<template>
    <div class="layout">
        <Layout> 
            <wHeader  class="cont-width"  ></wHeader>
            <Content class="cont-width" :style="{margin: '64px auto', minHeight: '500px'}" >

                <router-view></router-view>
            
            </Content>
            <wFooter></wFooter>
        </Layout>
    </div>
</template>
<script>
    import wHeader from './componets/header/index';
    import wFooter from './componets/footer/index';

    export default {
        data() {
            return {

            };
        },
        components:{
            wHeader,
            wFooter
        },
        mounted() {

        },
        beforeDestroy() {

        },
        methods: {

        }
    };
</script>