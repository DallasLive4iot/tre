

<template>
    <div class="green-box-2-mobile" >
        <h1 class="title3 segoeui-black-english-holly" style="margin-bottom:3vh;text-align: center;font-size: 3vh;">{{ children }}</h1>
        <h1 class="green-box-font" style="text-align: center;">- Find Great Deals</h1>
                <h1 class="green-box-font" style="text-align: center;">- Expand your Opportunities</h1>

        <h1 class="green-box-font" style="text-align: center;">- Manage your Schedule</h1>
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

</style>