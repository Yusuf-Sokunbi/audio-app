<template>
    <div class="p-3 grid grid-cols-2 gap-6 text-white ">
       <div v-for="playlist in playlists" :key="playlist.id" class="bg-blue-500 my-6  p-4 grid place-items-center" >
        <img :src="playlist.cover" alt="Image" class="w-[100px] h-[100px] rounded-full items-center">
     <audio controls>
       <source :src="playlist.audio" type="audio/mpeg">
     </audio> 
     <p class="font-bold text-xl capitalize ">{{ playlist.title }}</p>
     <p class="font-semibold text-lg capitalize">{{ playlist.artist }} <span class="italic">{{ playlist.year }}</span></p>
       </div>
    </div>
</template>
 
<script>
export default{
    name:'PlayList',
    props:['playlists'],
    

}</script>

https://github.com/Yusuf-Sokunbi/audio-app.git