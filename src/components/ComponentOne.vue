

<template>
    <div class="component-10-1" >
        <h1 class="title1 segoeui-black-english-holly-30px">{{ children }}</h1>
    </div>
</template>
<script>
export default {
    name: "ComponentOne", 
    props: ["children"],
};

</script>

<style>
.component-10-1 {
-webkit-backdrop-filter: blur (30px) brightness(115%); backdrop-filter: blur (30px) brightness(115%);
border-radius: 16px;
box-shadow: 3px 3px 10px #00000047;
margin-top: 20px;
margin-left: 5px;
margin-right: 5px;
margin-bottom: 5px;
height: auto;
width: auto;
background-color: var(--county-green);
resize: both;

}

.title1 {
    flex: 1;
    /* height: 36; */
    font-size: 5vh;
    letter-spacing: 0;
    line-height: 10px;
    margin-right: 10px;
    margin-left: 10px;
    color: white;
    resize: both;
}
</style>