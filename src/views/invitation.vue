<template>
  <div class="invitationPage">
   <img src="http://oi5j2489n.bkt.clouddn.com/4e80c5d2-9ca3-4c51-bf0a-1dc9ab1d3015.png" alt="" >
   <img src="http://oi5j2489n.bkt.clouddn.com/178d4d9f-b537-4fc3-8e35-6b07aa0c0d5c.png" alt="" >
   <img src="http://oi5j2489n.bkt.clouddn.com/7e04b564-69a1-4562-a663-2d31d07267c4.png" alt="" >
  </div>
</template>

<script>

export default {
  created () {
  },
  data () {
    return {
    }
  }
}
</script>
<style scoped lang="scss">
    .invitationPage{
        width:100%;
        height:100%;
        background: url('http://oi5j2489n.bkt.clouddn.com/97f494cf-0445-4796-b954-9943724b7f7f.png') no-repeat;
        background-size: 100%;
        background-color: #000;
        color:white;
        position: relative;
        img{
            top:0;
            left:0;
            right:0;
            bottom:0;
            position: absolute;
            width:100%;
            height:100%;
            opacity: 1;
            animation-name:myopcity2;
            animation-duration:.5s;
            animation-iteration-count:1;
            &:nth-child(1){
                animation-delay:.5s;
            }
            &:nth-child(2){
                animation-delay:1.5s;
            }
            &:nth-child(3){
                animation-name:myopcity;
                animation-duration:2s;
                animation-timing-function:linear;
                animation-iteration-count:999;
                animation-delay:.5s;
                animation-fill-mode : forwards;
            }
        }
    }
</style>
