<template>
    <div class="top-menu-button">
        <h1 class="title segoeui-regular-normal">{{ children }}</h1>
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
    border-radius: 200px;
    
}
.top-menu-button:hover{
    background-color: rgba(159, 255, 159, 0.178);

}
.title {

    flex: 1;
    height: 2vh;
    letter-spacing: 0;
    line-height: 0px;
    margin-right: 1.5vw;
    margin-left: 1.5vw;
    margin-top: 3vh;
    margin-bottom: .7vh;
    text-align: center;
    white-space: nowrap;
    opacity: 1;
    font-weight: 700;
    font-size: 2.8vh;
    justify-content: center;
    /* overflow: hidden; */
    color:#0a491c;
}</style>