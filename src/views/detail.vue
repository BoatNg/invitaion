<template>
  <div class="code">
    <img src="http://oi5j2489n.bkt.clouddn.com/1ef7ec4b-acc3-403a-9501-0598543803fb.png" alt="">
    <img src="http://oi5j2489n.bkt.clouddn.com/6b1c1789-b04c-45d6-a466-b06e6c294595.png" alt="">
    <img src="http://oi5j2489n.bkt.clouddn.com/666d3a28-8f42-4b0d-95e5-0e426ef5b13f.png" alt="">
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
            width:100%;
            height:100%;
            opacity: 1;
            animation-name:T_opcity;
            animation-duration:.5s;
            animation-delay: .5s;
            animation-iteration-count:1;
            &:nth-child(1){
                animation-name:myopcity;
                animation-duration:5s;
                animation-timing-function:linear;
                animation-iteration-count:999;
                opacity: 0;
            }
        }
    }
    @keyframes T_opcity
    {
        0%    {opacity: 1;}
        25%   {opacity: 0;}
        50%   {opacity: 1;}
        75%   {opacity: 0;}
        100%  {opacity: 1;}
    }
</style>
