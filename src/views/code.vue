<template>
  <div class="code">
   <img src="http://media.hkfsvip.com/72d2921b-0a29-4a4e-856d-7cc4f4ffd050.png" alt="" class="codeBox">
   <img src="http://oi5j2489n.bkt.clouddn.com/6b663e2a-98bc-4f22-ae28-dac2579e4554.png" alt="">
  </div>
</template>

<script>

export default {
  created () {

  },
  data () {
    return {
      img: 'http://oi5j2489n.bkt.clouddn.com/b32f0168-64de-4994-a675-8f55526be90c.png'
    }
  }
}
</script>
<style scoped lang="scss">
    .code{
        width:100%;
        height:100%;
        background: url('http://oi5j2489n.bkt.clouddn.com/df89229f-9f14-499a-8aa8-b895600696b5.png') no-repeat;
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
            &:nth-child(2){
                width:100%;
                height:100%;
                animation-name:myenter;
                animation-duration:2s;
                animation-timing-function:linear;
                animation-iteration-count:1;
                animation-fill-mode : forwards;
            }
        }
        .codeBox{
            width:80%;
            top:15%;
            left:10%;
            position: absolute;
        }
    }
</style>
