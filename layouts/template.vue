<template>
    <div style="overflow-x: hidden;">
        <ParallaxBG1 />
        <b-row>
            <b-col class="contentPortfolio" align-self="end">
                <Nuxt />
            </b-col>
            <b-col class="sideBarMenu d-none d-lg-block pr-0">
                <SideBarComponent />
            </b-col>
        </b-row>
    </div>
</template>

<style>
body {
    background-color: #000015;
    color: seashell;
}
.sideBarMenu{
    width: 300px;
    background-color: rgba(1, 7, 83, 0.6);
    position: fixed;
    height: 100%;
    box-shadow: 0px 1px 4px 0px white;
    -webkit-box-shadow: 0px 1px 4px 0px white;
}
.backSideBarMenu{
    width: 300px;
}
.contentPortfolio{
    width: 100%;
    border-left: 300px transparent solid;
}
@media (max-width: 976px) {
    .contentPortfolio{
        border-left: 0px transparent solid;
    }
}
</style>