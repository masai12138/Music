<template>
    <div class="footer">
        <ul class="footer-ul">
            <li @click="getMusic()">
                <i class="el-icon-service"></i>
                <span>音乐排行榜</span>
            </li>
            <li @click="getMine()">
                <i class="el-icon-star-off"></i>
                <span>我的收藏</span>
            </li>
        </ul>
    </div>
</template>

<script>
export default {
    name : 'Footer',
    data : function(){
        return {
        }
    },
    methods : {
        getMine : function(){
            this.$router.push('/about')
        },
        getMusic : function(){
            this.$router.push('/')
        }
    }
}
</script>
<style scoped>
.footer-ul li{
    width: 50%;
    height: 64px;
    list-style: none;
    float: left;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
}
.footer-ul li:hover{
    color: red;
}
.footer-ul{
    margin: 0;
    padding: 0;
    
}
</style>