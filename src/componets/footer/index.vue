<style scoped >
    .cont-width{
        width: 1200px;
        min-width: 1200px;
        margin: 0 auto;
    }
    .footer-wrap{
        height: 200px;
        background: #fff;
    }
    .t-border{
        border-top:1px solid #dddee1;
        padding-top: 20px;
    }
    .tooter-items{
        text-align: left;
    }
    .tooter-items a{
        color:#495060;
    }

</style>

<template>
    
    <Footer class="layout-footer-center footer-wrap">
        <div  class="cont-width t-border"  >

            <Row>
                <i-col span="12" >
                    <Row>
                        <i-col span="8" >
                            <!-- <Menu theme="light" >
                                    <MenuItem name="1">
                                        <Icon type="document-text"></Icon>
                                        文章管理
                                    </MenuItem>
                                    <MenuItem name="2">
                                        <Icon type="chatbubbles"></Icon>
                                        评论管理
                                    </MenuItem>
                            </Menu> -->
                            <div class="tooter-items" >
                                <h4>关注我们</h4>
                                <div>
                                    <Icon type="chatbubbles"></Icon>
                                    <a href="#">微信</a>
                                </div>                             
                                <div>
                                    <Icon type="at"></Icon>
                                    <a href="#">腾讯微博</a>                                    
                                    </div>
                                <div>
                                    
                                    <Icon type="at"></Icon>
                                    <a href="#">新浪微博</a>
                                </div>
                            </div>
                        </i-col>

                        <i-col  span="8"  >
                            <div class="tooter-items" >
                                <h4>加入我们</h4>
                                <div>
                                    <Icon type="chatbubbles"></Icon>
                                    <a href="#">微信</a>
                                </div>                             
                                <div>
                                    <Icon type="at"></Icon>
                                    <a href="#">腾讯微博</a>                                    
                                    </div>
                                <div>
                                    
                                    <Icon type="at"></Icon>
                                    <a href="#">新浪微博</a>
                                </div>
                            </div>
                        </i-col>
                        <i-col  span="8"  >
                            <div class="tooter-items" >
                                <h4>联系我们</h4>
                                <div>
                                    <Icon type="chatbubbles"></Icon>
                                    <a href="#">微信</a>
                                </div>                             
                                <div>
                                    <Icon type="at"></Icon>
                                    <a href="#">腾讯微博</a>                                    
                                    </div>
                                <div>
                                    
                                    <Icon type="at"></Icon>
                                    <a href="#">新浪微博</a>
                                </div>
                            </div>
                        </i-col>
                        
                    </Row>
                </i-col>

                <i-col span="12" >
                    2011-2016 &copy; TalkingData
                </i-col>
            </Row>
        
        </div>
    </Footer>

</template>

<script>
    
    export default {

    };
    

</script>