<style scoped >
   .wrap{
       padding-top: 30px;
   }
   .menu-wrap{
       /* text-align: right; */
   }
   .menu-title{
       padding: 14px 24px;
       border: none;
   }
    .page-content{
        padding-left: 30px;
    }
    .sub_sider{
        position: fixed;
        /* margin-left: 15px; */
        top: 94px;
        width: 200px;
        text-align: right;
    }
    .sub_cont{
        margin-left: 200px;
        padding-left: 30px;
    }
    .part{
        height: 500px;
    }
</style>
<template>
    <div class="wrap" > 
        <div class="sub_sider" >
            <div class="menu-title ivu-card-head" >
                <p>公司信息</p>
            </div>
            <Menu active-name="1-1" :style="{ width:'100%' }" > 
                <MenuItem name="1-1">
                    <a href="#company_charity">文章管理</a>
                </MenuItem>
                <MenuItem name="1-2">
                    <a href="#company_dev">评论管理</a>    
                
                </MenuItem>
                <MenuItem name="1-3">
                    <a href="#company_board">举报管理</a>
                </MenuItem> 
            </Menu>  
        </div>
        <div class="sub_cont" >
            <cardList title="文章管理" ></cardList>
            <cardList title="评论管理" ></cardList>
            <cardList title="举报管理" ></cardList>
            <!-- <div class="part" id="company_dev" >22</div>
            <div class="part" id="company_board" >33</div> -->
        </div>
            
    </div>
</template>

<script>
    import cardList from '../componets/card';
    export default {
        data(){
            return {

            }
        },
        components:{
            cardList
        }
    }
    
</script>