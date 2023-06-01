

<template>
    <div class="green-box-2" >
        <h1 class="title3 segoeui-black-english-holly-30px" style="margin-bottom:50px">{{ children }}</h1>
        <h1 class="green-box-font" style="justify-content: start;">- Simple Shipping Using TRS</h1>
        <h1 class="green-box-font" style="justify-content: start;">- Flexible Booking</h1>
        <h1 class="green-box-font">- High Quality Drivers</h1>
    </div>
</template>
<script>
export default {
    name: "ComponentOne", 
    props: ["children"],
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
width: 544px;
height: 243px;
justify-content: left;

}

.green-box-font {
    
    /* height: 36; */
    font: normal normal normal 25px/33px Segoe UI;
    font-size: 25px;
    letter-spacing: 0;
    line-height: 5px;
    margin-top: 40px;
    margin-right: 10px;
    margin-left: 10px;
    color: #277938;
    
}
</style>