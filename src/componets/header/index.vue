<style scoped >
    .ivu-layout-header{
        background: #fff;
        border: 1px solid #dddee1;
    }
    .layout-logo{
        width: 100px;
        height: 30px;
        border-radius: 3px;
        float: left;
        position: relative;
        top: 15px;
        left: 0px;
        margin-right: 100px;
    }
    .layout-logo img{
        width: 100%;
        height: 100%;
    }
    .ivu-menu{
        border:none;
    }
    .layout-ceiling-main{
        float: right;
    }
    .cont-width{
        width: 1200px;
        min-width: 1200px;
        margin: 0 auto;
    }
    .ivu-layout-header ul:after{
        height: auto;
    }

</style>

<template>
    <Header :style="{position: 'fixed', width: '100%', top:'0',zIndex:999}">
        <Menu class="cont-width"  mode="horizontal" theme="light" active-name="1">
            <div class="layout-logo">
                <img src="../../assets/img/logo.png" alt="">
            </div>
           
            <div class="layout-nav">
                <Submenu name="2">
                    <template slot="title">
                        <Icon type="stats-bars"></Icon>
                        公司信息
                    </template>
                    <MenuItem name="0-1">新增和启动</MenuItem>
                    <MenuItem name="0-2">活跃分析</MenuItem>
                    <MenuItem name="0-3">时段分析</MenuItem>
                </Submenu>
                <Submenu name="2">
                    <template slot="title">
                        <Icon type="stats-bars"></Icon>
                        企业文化
                    </template>
                    <MenuItem name="1-1">新增和启动</MenuItem>
                    <MenuItem name="1-2">活跃分析</MenuItem>
                    <MenuItem name="1-3">时段分析</MenuItem>
                </Submenu>
                <Submenu name="3">
                    <template slot="title">
                        <Icon type="stats-bars"></Icon>
                        业务体系
                    </template>
                    <MenuItem name="2-1">新增和启动</MenuItem>
                    <MenuItem name="2-2">活跃分析</MenuItem>
                    <MenuItem name="2-3">时段分析</MenuItem>
                    <MenuItem name="2-4">用户留存</MenuItem>
                    <MenuItem name="2-5">流失用户</MenuItem>
                </Submenu>
                <Submenu name="3">
                    <template slot="title">
                        <Icon type="stats-bars"></Icon>
                        投资者关系
                    </template>
                    <MenuItem name="3-1">新增和启动</MenuItem>
                    <MenuItem name="3-2">活跃分析</MenuItem>
                    <MenuItem name="3-3">时段分析</MenuItem>
                    <MenuItem name="3-4">用户留存</MenuItem>
                    <MenuItem name="3-5">流失用户</MenuItem>
                </Submenu>

            </div>
            <div class="layout-ceiling">
                <div class="layout-ceiling-main">
                    <a href="#">简</a> |
                    <a href="#">繁</a> |
                    <a href="#">EN</a> 
                </div>
            </div>

        </Menu>
    </Header>
</template>
<script>
    export default{
        data(){
            return {
                randomMovieList:[]
            }
        }
    }
</script>