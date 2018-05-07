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
        cursor: pointer;
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
    .layout-logo .ivu-menu-item-active , .layout-logo .ivu-menu-item-active:hover{
        border: none
    }
</style>

<template>
    <Header :style="{position: 'fixed', width: '100%', top:'0',zIndex:999}">
        <Menu 
            class="cont-width"  
            mode="horizontal" 
            theme="light" 
            :active-name="name"  
            @on-select="changeRouter" 
            ref="header_menu"
        >
            <div class="layout-logo" @click="tohome" >
                <img src="../../assets/img/logo.png" alt="玩咖">
            </div>
           
            <div class="layout-nav">
                <MenuItem name="infos">
                    <Icon type="stats-bars"></Icon>
                    公司信息                        
                    <!-- <router-link to="/" >公司信息</router-link> -->
                </MenuItem>
                <MenuItem name="culture">
                    <Icon type="stats-bars"></Icon>
                    企业文化

                </MenuItem>
                <MenuItem name="system">
                    <Icon type="stats-bars"></Icon>
                    业务体系
                </MenuItem>

                <MenuItem name="investor">
                    <Icon type="stats-bars"></Icon> 
                    投资者关系                   
                </MenuItem>
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
            return {};
        },
        computed:{
            name(){
                return this.$route.name;
            }
        },
        methods:{
            // 跳转路由
            changeRouter(name){

                this.$router.push({
                    name
                });
            },
            tohome(){

                this.$router.push({
                    name:'index'
                });

                // 更新导航菜单选中状态
                this.$nextTick(() => {
                    this.$refs.header_menu.updateActiveName();
                });
            }
        }
    };
</script>