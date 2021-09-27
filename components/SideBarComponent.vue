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
        
        <div class="sideBarMain pt-5 pt-4 px-3">
            <b-img class="mt-3 mb-4" src="https://picsum.photos/200/200/?image=41" fluid center thumbnail rounded="circle" alt="Foto de Perfil"></b-img>
            <h4 style="text-align: center;">{{ nombre }}</h4>
            <h5 style="text-align: center;">{{ apellido }}</h5>
            <b-row class="OptionsMenu mt-5">
                <b-col v-for="navOption in navOptions" v-bind:key="navOption.id" cols="12">
                    <div class="Option">
                        <b-icon :icon="navOption.icon"></b-icon> {{ navOption.title }}
                    </div>
                </b-col>
            </b-row>
            <!-- <b-button v-b-toggle.sidebar-variant>Toggle Sidebar</b-button> Boton de menu bar lateral-->
        </div>
    </div>
</template>

<script>

import { BIcon, BIconHouseFill, BIconPersonFill, BIconLightning, BIconInboxes, BIconGithub, BIconLinkedin } from 'bootstrap-vue'


export default {
    data(){
        return {
            nombre: "Jhon Eymar",
            apellido: "Rodríguez Arteaga",
            navOptions: [
                {
                    title: "Inicio",
                    icon: "house-fill"
                },
                {
                    title: "Sobre mi",
                    icon: "person-fill"
                },
                {
                    title: "Habilidades",
                    icon: "lightning"
                },
                {
                    title: "Contacto",
                    icon: "inboxes"
                }
            ]
        }
    },
    components: {
        BIcon,
        BIconHouseFill,
        BIconPersonFill,
        BIconLightning,
        BIconInboxes
    },
}
</script>

<style scoped>

.Option{
    width: 100%;
    font-size: 20px;
    cursor: pointer;
    font-family: sans-serif;
    color: #b8fffc;
    letter-spacing: 1px;
    word-spacing: -1.8px;
    font-style: normal;
    text-transform: lowercase;
    outline: none;
    padding-left: 14px;
    padding-bottom: 4px;
    margin-bottom: 5px;
}
.OptionActive, .Option:hover{
    -webkit-box-shadow: inset 36px 0px 38px -34px #b8fffc, -4px 0px 0px 0px #b8fffc; 
    box-shadow: inset 36px 0px 38px -34px #b8fffc, -4px 0px 0px 0px #b8fffc;
    border-radius: 0px 2px 2px 0px;
    color: white;
    border-left: 3px solid transparent;
}

</style>