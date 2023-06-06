

<template>
    <div class="about-us" style="justify-content: center;">
        <img src="@/assets/ShakingHands.png" style="height:9vh;margin-top: 4vh;" />
        <h1 class="about-us-font">TRE is a company that has a strong spirit of cooperation, hence we provide partnership. Helps you earn passive income.</h1>


    </div>
</template>
<script>
export default {
    name: "AboutUs", 

};

</script>

<style>
.about-us{
width: 20vw;
height: 44vh;
/* UI Properties */
background: #ffffff44 0% 0% no-repeat padding-box;
box-shadow: 3px 3px 6px #00000029;
border-radius: 60px;
opacity: 1;
backdrop-filter: blur(30px);
-webkit-backdrop-filter: blur(30px);
transition: 1s;
}

.about-us-font{
    text-align: center;
font: normal normal normal 2.6vh Segoe UI;
letter-spacing: 0px;
color: #FFFFFF;
opacity: 1;
margin-top: 6vh;
margin-left: 3vh;
margin-right:3vh;
transition: 1s;
}
.about-us:hover{
    color: aqua;
    transform: scale(1.1);
}

</style>