<template>
  <iframe 
    :width="width" 
    :height="height" 
    :src="url+yid" 
    frameborder="0" 
    allow="autoplay; encrypted-media" 
    allowfullscreen>
  </iframe>
</template>
<script>
export default {
  data(){
    return{
      url:"https://www.youtube.com/embed/"
    }
  },
  props:{
    width:String,
    height:String,
    yid:String,
  }
}
</script>
