<template>
    <div>
        <div class="sideBarMain pt-5 px-1">
            <b-img class="mt-3 mb-4" src="https://picsum.photos/200/200/?image=41" fluid center thumbnail rounded="circle" alt="Foto de Perfil"></b-img>
            <h4 style="text-align: center; font-family: 'Roboto Mono';">{{ nombre }}</h4>
            <h5 style="text-align: center; font-family: 'Roboto Mono';">{{ apellido }}</h5>

            <div class="social">
                <a href="https://github.com/GatekoNeko141" target="_blank" style="cursor: pointer; color: white;">
                    <b-icon icon="github" v-b-tooltip.hover.bottom="'GitHub'"></b-icon>
                </a>
                <a href="https://www.linkedin.com/in/gko-rodriguez/" target="_blank" style="cursor: pointer; color: white;">
                    <b-icon icon="linkedin" v-b-tooltip.hover.bottom="'LinkedIn'"></b-icon>
                </a>
                <a href="mailto:jhon1995jera@gmail.com" target="_blank" style="cursor: pointer; color: white;">
                    <b-icon icon="envelope-fill" v-b-tooltip.hover.bottom="'Enviar Correo'"></b-icon>
                </a>
            </div>

            <b-row class="OptionsMenu mt-5">
                <b-col v-for="navOption in navOptions" v-bind:key="navOption.id" cols="12">
                    <div class="Option">
                        <b-icon style="width: 30px;" :icon="navOption.icon"></b-icon>
                        <span>{{ navOption.title }}</span>
                    </div>
                </b-col>
            </b-row>
            
        </div>
    </div>
</template>

<script>

import {
    BIcon,
    BIconHouseFill,
    BIconPersonFill,
    BIconLightning,
    BIconInboxes,
    BIconGithub,
    BIconLinkedin,
    BIconEnvelopeFill
} from 'bootstrap-vue'


export default {
    data(){
        return {
            nombre: "John Eymar",
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
        BIconInboxes,
        BIconGithub,
        BIconLinkedin,
        BIconEnvelopeFill
    },
}
</script>

<style scoped>

.Option{
    width: 100%;
    font-size: 20px;
    cursor: pointer;
    font-family: 'Roboto Mono';
    color: #b8fffc;
    font-weight: 300;
    letter-spacing: 1px;
    word-spacing: -1.8px;
    font-style: normal;
    text-transform: lowercase;
    outline: none;
    padding-left: 14px;
    padding: 6px 0px;
    margin-bottom: 7px;
}
.OptionActive, .Option:hover{
    -webkit-box-shadow: inset 36px 0px 38px -34px #b8fffc, -4px 0px 0px 0px #b8fffc; 
    box-shadow: inset 36px 0px 38px -34px #b8fffc, -4px 0px 0px 0px #b8fffc;
    border-radius: 0px 2px 2px 0px;
    color: white;
    border-left: 3px solid transparent;
}
.social{
    padding-top: 10px;
    text-align: center;
    font-size: 25px;
    letter-spacing: 10px;
}

</style>