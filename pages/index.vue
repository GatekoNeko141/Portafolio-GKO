<template>
    <div class="content">
        <b-container class="cont">
            <inicio />
        </b-container>

        <b-container class="cont">
            <about />
        </b-container>
    </div>
</template>

<script>
import inicio from "../components/content/inicio";
import about from "../components/content/about";
export default {
    layout: "template",
    components:{
        inicio,
        about
    }
}
</script>

<style scoped>
.content{
    font-family: 'Roboto Mono';
    color: #d9ebff;
    letter-spacing: 1.5px;
    word-spacing: -1.8px;
}
.cont{
    border: 1px transparent solid;
    height: 100vh;
}
</style>
