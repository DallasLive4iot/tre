

<template>
    <div class="green-box-2" >
        <h1 class="title3 segoeui-black-english-holly-30px" style="margin-bottom:3vh;margin-left: 3vw;">{{ children }}</h1>
        <h1 class="green-box-font" style="justify-content: start;">- Simple Shipping Using TRS</h1>
        <h1 class="green-box-font" style="justify-content: start;">- Flexible Booking</h1>
        <h1 class="green-box-font">- High Quality Drivers</h1>
        <img v-show="!mobile" src="@/assets/PackagePerson.png" style="height:13vh; position: absolute; top: 13vh; left: 20vw;resize: both;" />
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
      if(this.windowWidth <= 750){
        this.mobile = true;
        return
      }
      this.mobile = false;
    },
  }
};

</script>

<style>
.green-box-2 {
    background: #e3f3e7 0% 0% no-repeat padding-box;
box-shadow: 3px 3px 10px #00000047;
border-radius: 30px;
opacity: 1;
backdrop-filter: blur(30px);
-webkit-backdrop-filter: blur(30px);
width: 28vw;
height: 25vh;
justify-content: left;
resize: both;

}

.green-box-font {
    
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