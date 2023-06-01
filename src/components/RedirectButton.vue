<template>
    <div class="top-menu-button">
        <h1 class="title segoeui-regular-normal-dove-gray-25px">{{ children }}</h1>
    </div>
</template>
<script>
export default {

    name: "TopMenuButton",
    props: ["children"],
};
</script>
<style>
-top-menu-button {
    display: flex;
    height: 39px;
    width: 5;
}

.title {

    flex: 1;
    height: 25px;
    letter-spacing: 0;
    line-height: 0px;
    margin-right: 40px;
    margin-top: 0px;
    text-align: center;
    white-space: nowrap;
    opacity: 0.7;
    font-weight: 100;
    font-size: 25px;
    justify-content: center;
}</style>