<template>
    <div class="correction">
        <ParallaxBG1 />
        <b-row>
            <b-col lg="3" class="bg-dark">
                <b-row>
                    <b-col></b-col>
                    <b-col cols="10">
                        <SideBarComponent />
                    </b-col>
                </b-row>
            </b-col>
            <b-col lg="9">
                <Nuxt />
            </b-col>
        </b-row>
    </div>
</template>

<style>
.correction{
    overflow-x: hidden;
}
</style>