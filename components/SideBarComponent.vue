<template>
    <div>
        <b-sidebar id="sidebar-variant" title="Sidebar" bg-variant="dark" text-variant="light" shadow>
        <div class="px-3 py-2">
            <p>
            Cras mattis consectetur purus sit amet fermentum. Cras justo odio, dapibus ac facilisis
            in, egestas eget quam. Morbi leo risus, porta ac consectetur ac, vestibulum at eros.
            </p>
            <b-img src="https://picsum.photos/400/400/?image=54" fluid thumbnail></b-img>
        </div>
        </b-sidebar>
        
        <div class="sideBarMain pt-5 pt-4 px-4">
            <b-img class="mt-3 mb-5" src="https://picsum.photos/200/200/?image=41" fluid center thumbnail rounded="circle" alt="Foto de Perfil"></b-img>
            <b-row>
                <b-col cols="12">
                    <div class="Option">inicio</div>
                </b-col>
                <b-col cols="12">
                    <div class="OptionActive Option">inicio</div>
                </b-col>
                <b-col cols="12">
                    <div class="Option">inicio</div>
                </b-col>
            </b-row>
            <!-- <b-button v-b-toggle.sidebar-variant>Toggle Sidebar</b-button> Boton de menu bar lateral-->
        </div>
    </div>
</template>

<style scoped>

.Option{
    font-size: 24px;
    cursor: pointer;
    font-family: Tahoma, Geneva, sans-serif;
    color: #b8fffc;
    letter-spacing: 1px;
    word-spacing: -1.8px;
    font-weight: 400;
    font-style: normal;
    font-variant: small-caps;
    text-transform: lowercase;
    outline: none;
    padding-left: 14px;
    padding-bottom: 4px;
    margin-bottom: 5px;
}
.OptionActive, .Option:hover{
    -webkit-box-shadow: inset 10px 0px 17px -4px #c5caca, -2px 0px 4px -2px #b8fffc; 
    box-shadow: inset 10px 0px 17px -4px #b8fffc, -2px 0px 4px -2px #b8fffc;
    border-radius: 2px;
    color: white;
}
.Option::before{
    content: '';
    background-color: transparent;
    position: absolute;
    top: 1px;
    left: 6px;
    width: 4px;
    height: 38px;
}
.OptionActive::before, .Option:hover ~ .Option::before{
    background-color: #b8fffc;
}

</style>