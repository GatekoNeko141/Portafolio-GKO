<template>
  <b-container>
    <div class="pr-3">
      <h1 class="center">Sobre mi</h1>
      <hr class="my-4">

      <div>
        <b-row class="m-0">
          <b-col md="12" lg="6" class="align-c-c">
            <p class="center fz-20">
              Desarrollador de software, apasionado por la tecnologia desde 2013, dedicado
              al mundo del desarrollo de software, capacidad profesional para encausar y
              resolver problemas, habil en toma de desiciones, trabajo en equipo, cuento
              con experiencia en proyectos de ambito web, dedicado, responsable y
              colaborador.
            </p>
          </b-col>
          <b-col md="12" lg="6" class="p-0">
            <div class="tilesSkill align-c-c">

              <div class="itemSkill" v-for="skill in skills" v-bind:key="skill.id">
                <a class="linkSkill" :href="skill.href" target="blank" >
                  <div class="skill pt-2 mx-2 my-2">
                    <div class="img-skill mx-5 align-c-c">
                      <b-img v-bind:src="require(`~/assets/img/${skill.img}`)" alt=""></b-img>
                    </div>
                    <p class="center m-0">{{ skill.name }}</p>
                  </div>
                </a>
              </div>

            </div>
          </b-col>
        </b-row>
      </div>
    </div>
    
  </b-container>
</template>

<script>

export default {
  data(){
    return {
      nombre: "John Eymar",
      skills: [
        {
          id: 1,
          name: "HTML",
          img: "skill-html.svg",
          href: "https://developer.mozilla.org/es/docs/Web/HTML"
        },
        {
          id: 2,
          name: "CSS",
          img: "skill-css.svg",
          href: "https://developer.mozilla.org/es/docs/Web/CSS"
        },
        {
          id: 3,
          name: "JavaScript",
          img: "skill-js.svg",
          href: "https://developer.mozilla.org/es/docs/Web/JavaScript"
        },
        {
          id: 4,
          name: "NodeJS",
          img: "skill-node.png",
          href: "https://nodejs.org/es/"
        },
        {
          id: 5,
          name: "React",
          img: "skill-react.svg",
          href: "https://es.reactjs.org"
        },
        {
          id: 6,
          name: "Vue",
          img: "skill-vue.svg",
          href: "https://vuejs.org"
        },
        {
          id: 7,
          name: "Electron",
          img: "skill-electron.svg",
          href: "https://www.electronjs.org/es/"
        },
        {
          id: 8,
          name: "Next",
          img: "skill-next.png",
          href: "https://nextjs.org"
        },
        {
          id: 9,
          name: "Nuxt",
          img: "skill-nuxt.svg",
          href: "https://nuxtjs.org"
        },
        {
          id: 10,
          name: "PHP",
          img: "skill-php.svg",
          href: "https://www.php.net/manual/es/intro-whatis.php"
        },
        {
          id: 11,
          name: "C#",
          img: "skill-csharp.svg",
          href: "https://docs.microsoft.com/en-us/dotnet/csharp/"
        },
        {
          id: 12,
          name: "Git",
          img: "skill-git.svg",
          href: "https://es.wikipedia.org/wiki/Git"
        }
      ]
    }
  },
  methods:{
    //
  },
  created () {
    //
  },
  destroyed () {
    //
  }
}
</script>

<style scoped>
.itemSkill{width: 157px;}
.tilesSkill{flex-wrap: wrap;}
.skill{
  border-radius: 6px;
  background-color: var(--color-02);
  border: 1px var(--color-03) solid;
}
.skill:hover{
  border: 1px var(--white) solid;
}
.linkSkill{text-decoration: none;}
.img-skill{height: 60px;}
.skill p{color: var(--white);}
.img-skill img{height: 100%;}

</style>
