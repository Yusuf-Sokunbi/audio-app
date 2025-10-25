<template>
    <div class="p-2 grid grid-cols-2 md:grid-cols-4 gap-2 text-white ">
       <div v-for="playlist in playlists" :key="playlist.id" class="bg-blue-500 my-6  p-4 grid place-items-center" >
        <img :src="playlist.cover" alt="Image" class="w-[100px] h-[100px] rounded-full items-center">
     <audio controls class="w-full mx-2">
       <source :src="playlist.audio" type="audio/mpeg">
     </audio> 
     <p class=" font-semibold md:font-bold text-sm md:text-xl capitalize ">{{ playlist.title }}</p>
     <p class="font-semibold text-xs capitalize">{{ playlist.artist }} <span class="italic">{{ playlist.year }}</span></p>
       </div>
    </div>
</template>
 
<script>
export default{
    name:'PlayList',
    props:['playlists'],
    

}</script>