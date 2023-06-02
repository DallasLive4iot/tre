<template>
    <div class="top-menu-button">
        <h1 class="title segoeui-regular-normal-dove-gray">{{ children }}</h1>
    </div>
</template>
<script>
export default {

    name: "TopMenuButton",
    props: ["children"],
};
</script>
<style>
.top-menu-button {
    display: flex;
    height: fit-content;
    /* width: 5vh; */
    /* background-color: red; */
    
}

.title {

    flex: 1;
    height: 2vh;
    letter-spacing: 0;
    line-height: 0px;
    margin-right: 1.5vw;
    margin-left: 1.5vw;
    margin-top: 3vh;
    text-align: center;
    white-space: nowrap;
    opacity: 0.7;
    font-weight: 100;
    font-size: 2.5vh;
    justify-content: center;
    /* overflow: hidden; */
}</style>