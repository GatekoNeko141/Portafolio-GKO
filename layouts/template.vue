<template>
    <div style="overflow-x: hidden;">
        <ParallaxBG1 />
        <b-row>
            <b-col lg="2"></b-col>
            <b-col lg="2" class="sideBarMenu d-none d-lg-block pr-0">
                <SideBarComponent />
            </b-col>
            <b-col cols="12" lg="10" align-self="end">
                <Nuxt />
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
    background-color: rgba(0, 4, 56, 0.6);
    position: fixed;
    height: 100%;
}
</style>