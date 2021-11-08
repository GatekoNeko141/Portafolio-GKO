<template>
    <div style="overflow-x: hidden;">
        <ParallaxBG1 />
        <b-navbar toggleable type="dark" variant="transparent" class="navbar">
            <b-navbar-brand href="#">&lt;John Dev/&gt;</b-navbar-brand>
            <b-button variant="outline-light" v-b-toggle.sidebar-variant>
                <b-icon icon="list"></b-icon>
            </b-button>
        </b-navbar>

        <b-row>
            <b-col class="contentPortfolio" align-self="end">
                
                <b-sidebar id="sidebar-variant" bg-variant="transparent" text-variant="light" shadow width="100%" header-class="sidebar-variant" body-class="sidebar-variant">
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
                        <b-col v-for="navOption in navOptions" v-bind:key="navOption.id" cols="11">
                            <div class="Option">
                                <b-icon style="width: 30px;" :icon="navOption.icon"></b-icon>
                                <span>{{ navOption.title }}</span>
                            </div>
                        </b-col>
                    </b-row>
                </b-sidebar>

                <Nuxt />
            </b-col>

            <b-col class="sideBarMenu pr-0">
                <SideBarComponent />
            </b-col>
        </b-row>
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
    BIconEnvelopeFill,
    BIconList
} from 'bootstrap-vue'


export default {
    data(){
        return {
            nombre: "John Eymar",
            apellido: "Rodríguez Arteaga",
            navOptions: [
                {
                    title: "Bienvenidos",
                    icon: "house-fill"
                },
                {
                    title: "Sobre mi",
                    icon: "person-fill"
                },
                {
                    title: "Portafolio",
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
        BIconEnvelopeFill,
        BIconList
    },
}
</script>

<style scope>
body {
    background-color: #000015;
    color: seashell;
}
.sideBarMenu{
    display: block;
    width: 300px;
    background-color: rgba(1, 7, 83, 0.6);
    position: fixed;
    height: 100%;
    box-shadow: 0px 1px 4px 0px white;
    -webkit-box-shadow: 0px 1px 4px 0px white;
}
.contentPortfolio{
    width: 100%;
    border-left: 300px transparent solid;
}
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
.OptionsMenu{
    overflow: hidden;
    width: 100%;
    margin: auto;
}
.sidebar-variant{
    background-color: rgba(1, 7, 83, 0.95) !important;
}
.navbar{
    display: none;
    position: fixed;
    z-index: 10;
    width: 100%;
    background-color: rgba(1, 7, 83, 0.95) !important;
    font-family: 'Roboto Mono';
}
@media (max-width: 976px) {
    .contentPortfolio{
        border-left: 0px transparent solid;
    }
    .sideBarMenu{display: none;}
    .navbar{display: flex;}
}
</style>