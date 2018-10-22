<template>
  <div class="mainPage">
    <img src="http://oi5j2489n.bkt.clouddn.com/7c6a413a-4eb3-49c8-95de-0659405cca82.png" alt="" v-if="showMain">
    <img src="http://oi5j2489n.bkt.clouddn.com/6783d5ad-6875-42da-be7b-c4d1c61a0f4a.png" alt="" v-else>
    <img src="http://oi5j2489n.bkt.clouddn.com/6d4c0314-b18b-4419-8dac-b145e457245c.png" alt="" class="o" v-if="showMain">
    <img src="http://oi5j2489n.bkt.clouddn.com/6bf84ef0-899f-4e79-b356-2817d34bfe22.png" alt="" class="r" v-if="showMain">
    <img src="http://oi5j2489n.bkt.clouddn.com/3fce5d9f-1a8b-4031-a47f-cc0a8c9fb0c1.png" alt="" class="a" v-if="showMain">
    <img src="http://oi5j2489n.bkt.clouddn.com/1a070fb2-a0af-4ba5-b958-29ad5acd234e.png"  alt=""  v-if="starShow">
    <img src="http://oi5j2489n.bkt.clouddn.com/b0459a27-6b2a-4ae1-8451-789876f94468.png"  alt="" v-else>
    <img src="http://oi5j2489n.bkt.clouddn.com/d470eb6b-ad13-4f0d-b2c3-7c1a45eac040.png" alt="" v-if="fwShow">
    <img src="http://oi5j2489n.bkt.clouddn.com/cf53fa1d-5537-4502-ae58-7a935b1e11e8.png" alt="" v-else>
    <img src="http://oi5j2489n.bkt.clouddn.com/f504fe93-7e30-4d88-80f1-7b45fbdec331.png" alt="" class="logo">
  </div>
</template>

<script>

export default {
  created () {
    setTimeout(() => {
      this.showContent()
    }, 400)
    setTimeout(() => {
      this.starShow = !this.starShow
    }, 350)
    setTimeout(() => {
      this.fwShow = !this.fwShow
    }, 300)
  },
  data () {
    return {
      showMain: false,
      starShow: false,
      fwShow: false
    }
  },
  methods: {
    showContent () {
      let p = setInterval(() => {
        this.showMain = !this.showMain
      }, 200)
      setTimeout(() => {
        clearTimeout(p)
        this.showMain = true
      }, 800)
    }
  }
}
</script>
<style scoped lang="scss">
    .mainPage{
        width:100%;
        height:100%;
        background: url('http://oi5j2489n.bkt.clouddn.com/6429c56d-629f-414f-aa02-fc430879f7cb.png') no-repeat;
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
        }
        .o{
            animation-name: O_opcity;
            animation-duration:.1s;
            animation-fill-mode : forwards;
            animation-iteration-count:999;
            animation-delay: 1s;
            opacity: 1;
        }
        .r{
            animation-name: R_opcity;
            animation-duration:2s;
            animation-timing-function:linear;
            animation-iteration-count:999;
            animation-delay: .6s;
            opacity: 1;
        }
        .a{
            animation-name: O_opcity;
            animation-duration:.1s;
            animation-fill-mode : forwards;
            animation-iteration-count:999;
            animation-delay: 1.5s;
            opacity: 1;
        }
        .logo{
            animation-name: myopcity;
            animation-duration:5s;
            animation-timing-function:linear;
            animation-iteration-count:999;
            opacity: 0;
        }
        @keyframes R_opcity
        {
            0% { opacity: 0.3;}
            10% { opacity: 0.7;}
            20%{opacity: 0;}
            30%{opacity: 0.5;}
            40%{opacity: 0;}
            60%{opacity: 0;}
            70%{opacity: 0.5;}
            80%{opacity: 0;}
            100%{opacity: 0;}
        }
        @keyframes O_opcity
        {
            0%   {opacity: 0.3;}
            100% {opacity: 0.1;}
        }
    }
</style>
