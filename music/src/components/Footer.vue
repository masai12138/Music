<template>
    <div class="footer">
        <ul class="footer-ul">
            <li >

            </li>
            <li >

            </li>
        </ul>
        <div class="button">

        </div>
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
 
    }
}
</script>
<style scoped>
.footer{
    width: 100%;
}     
.footer-ul{
     width: 40%;
     height: 64px;
     background-color: blue;
     float: left;
}  
.button{
    width: 60%;
    height: 64px;
    background-color: red;
    float: left;
    margin: 0;
}
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