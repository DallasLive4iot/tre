

<template>
    <div class="green-box-3" >
        <h1 class="title3 segoeui-black-english-holly-30px" style="margin-bottom:3vh;margin-left: 3vw;">{{ children }}</h1>
        <h1 class="green-box-font">- Find Great Deals</h1>
        <h1 class="green-box-font">- Expand your Opportunities</h1>
        <h1 class="green-box-font">- Manage your Schedule</h1>
        <img src="@/assets/CaresPerson.png" v-show="!mobile" style="height:12vh; position: absolute; top: 14vh; left: 22vw;resize: both;" />
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
      if(this.windowWidth <= 1000){
        this.mobile = true;
        return
      }
      this.mobile = false;
    },
  }
};

</script>

<style>
.green-box-3 {
background: #e3f3e7 0% 0% no-repeat padding-box;
box-shadow: 3px 3px 10px #00000047;
border-radius: 30px;
opacity: 1;
backdrop-filter: blur(30px);
-webkit-backdrop-filter: blur(30px);
width: 28vw;
height: 25vh;
resize: both;
}


</style>