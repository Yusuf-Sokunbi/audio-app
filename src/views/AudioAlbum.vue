<template>
    <div>
      <PlayList :playlists="albums" />
 

      
    </div>
</template>

<script>
import {albums} from '../album.js'
import PlayList from '@/components/PlayList.vue';
export default{
 name:"AudioAlbum",
 data(){
    return{
        albums
    }
 },
 components:{
  PlayList
 }
}
</script>