

<template>
    <div class="green-box-2-mobile" >
        <h1 class="title3 segoeui-black-english-holly" style="margin-bottom:3vh;margin-left: 3vw;font-size: 3vh;">{{ children }}</h1>
        <h1 class="green-box-font-mobile" style="justify-content: start;">- Simple Shipping Using TRS</h1>
        <h1 class="green-box-font-mobile" style="justify-content: start;">- Flexible Booking</h1>
        <h1 class="green-box-font-mobile">- High Quality Drivers</h1>
    </div>
    
</template>
<script>
export default {
    name: "ComponentOne", 
    props: ["children"],
    created(){
    window.addEventListener("resize",this.checkScreen);
    this.checkScreen();
  },
  methods:{
    checkScreen(){
      this.windowWidth = window.innerWidth;
      if(this.windowWidth <= 700){
        this.mobile = true;
        this.windowed = false;
        this.desktop = false;
        return
      }
      else if(this.windowWidth <=1000){
        this.windowed = true;
        this.mobile = false;
        this.desktop = false;
        return
      }
      this.windowed = false;
      this.mobile = false;
      this.desktop = true;
    },
  }
};

</script>

<style>
.green-box-2-mobile {
    background: #e3f3e7 0% 0% no-repeat padding-box;
box-shadow: 3px 3px 10px #00000047;
border-radius: 30px;
opacity: 1;
backdrop-filter: blur(30px);
-webkit-backdrop-filter: blur(30px);
width: 85vw;
height: 25vh;
justify-content: left;
resize: both;

}

.green-box-font-mobile {
    
    /* height: 36; */
    font: normal normal normal 3vh Segoe UI;
    letter-spacing: 0;
    line-height: 5vh;
    margin-top: -2vh;
    /* margin-right: 5vh; */
    margin-left: 3vw;
    color: #277938;
    resize: both;
    text-align: left;
    white-space: nowrap;
    overflow:clip;
    
    
}
</style>