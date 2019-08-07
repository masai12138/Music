<template>
  <div class="home">
    <Song class="song"></Song>
  </div>
</template>
<script>
import Song from '@/components/Song.vue'
export default {
  data : function(){
    return {

    }
  },
  components :{
    Song
  }
}
</script>
<style scoped>
.song{
  overflow: hidden;
}
</style>

