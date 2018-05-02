<style scoped >
    .ivu-layout-header{
        background: #fff;
    }
    .layout-logo{
        width: 100px;
        height: 30px;
        border-radius: 3px;
        float: left;
        position: relative;
        top: 15px;
        left: 20px;
        margin-right: 100px;
    }
    .layout-logo img{
        width: 100%;
        height: 100%;
    }
    .ivu-menu{
        border:none;
    }

</style>

<template>
    <Header :style="{position: 'fixed', width: '100%'}">
        <Menu mode="horizontal" theme="light" active-name="1">
            <div class="layout-logo">
                <img src="../../assets/img/logo.png" alt="">
            </div>
            <div class="layout-nav">
                <MenuItem name="1">
                    <Icon type="ios-navigate"></Icon>
                    Item 1
                </MenuItem>
                <MenuItem name="2">
                    <Icon type="ios-keypad"></Icon>
                    Item 2
                </MenuItem>
                <MenuItem name="3">
                    <Icon type="ios-analytics"></Icon>
                    Item 3
                </MenuItem>
                <Submenu name="3">
                    <template>
                        <Icon type="stats-bars"></Icon>
                        统计分析
                    </template>
                    <MenuItem name="3-4">用户留存</MenuItem>
                    <MenuItem name="3-5">流失用户</MenuItem>

                </Submenu>
            </div>
            <div>
                
            </div>
        </Menu>
    </Header>
</template>
<script>
    export default{

    }
</script>