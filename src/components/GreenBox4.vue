

<template>
    <div class="green-box-4" >
        <h1 class="title3 segoeui-black-english-holly-30px" style="margin-bottom:50px">{{ children }}</h1>
        <h1 class="green-box-font">- Safe & Secure</h1>
        <h1 class="green-box-font">- Better Control of your Vehicle</h1>
        <h1 class="green-box-font">- Become a Preferred Driver</h1>
    </div>
</template>
<script>
export default {
    name: "ComponentOne", 
    props: ["children"],
};

</script>

<style>
.green-box-4 {
    background: #e3f3e7 0% 0% no-repeat padding-box;
box-shadow: 3px 3px 10px #00000047;
border-radius: 30px;
opacity: 1;
backdrop-filter: blur(30px);
-webkit-backdrop-filter: blur(30px);
width: 544px;
height: 243px;

}


</style>