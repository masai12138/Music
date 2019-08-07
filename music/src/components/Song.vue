<template>
    <div class="main">
        <ul class="main-ul">
            <li>1</li>
            <li>2</li>
            <li>3</li>
            <li>4</li>
            <li>5</li>
            <li>6</li>
        </ul>
    </div>
</template>

<style scoped>
.main-ul li{
    width: 100%;
    height: 93px;
    background-color: brown;
    list-style: none;
    margin-top: 6px;
}
.main-ul{
    margin: 0;
    padding: 0;
}
</style>

<script>
import axios from "axios";
export default {
    name : 'Song',
    data : function(){
        return {
            Music : null,
        }
    },
    created : function(){
        let that = this
        console.log("create")
        axios.get(`https://api.apiopen.top/musicRankings`)
        .then(function(response){
            console.log(response)
            if (response.status !== 200) {
                console.log('error, code: ', error.code, ', msg: ', error.msg)
                return;
            }
            let MusicArray = response.data
            that.Music = MusicArray[0]
        })
    }
}
</script>


