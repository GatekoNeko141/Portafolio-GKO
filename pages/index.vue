<template>
    <div class="content">
        <b-container id="inicio" class="container_1">
            <h1>&lt;John Dev/&gt;</h1>
            <div class=fakeMenu>
                <div class="fakeButtons fakeClose"></div>
                <div class="fakeButtons fakeMinimize"></div>
                <div class="fakeButtons fakeZoom"></div>
            </div>
            <div class="fakeTerminal">
                <h2 class="line1">¡Saludos! Bienvenido a mi portafolio web<span class="cursor1">_</span></h2>
                <h2 class="line2">Soy <strong>John Eymar Rodríguez Arteaga</strong><span class="cursor2">_</span></h2>
                <h2 class="line3">Programador UI/UX.<span class="cursor3">_</span></h2>
                <h2 class="line4">$<span class="cursor4">_</span></h2>
            </div>
        </b-container>

        <b-container class="container_2">
            sobre mi?
        </b-container>
    </div>
</template>

<script>
export default {
    layout: "template"
}
</script>

<style scoped>

.content{
    font-family: 'Roboto Mono';
    color: #d9ebff;
    letter-spacing: 1.5px;
    word-spacing: -1.8px;
}
.container_1, .container_2{
    border: 1px transparent solid;
    height: 100vh;
}
.container_1 h1{
    font-size: 49px;
    margin-top: 31vh;
    margin-bottom: 1em;
    text-shadow: 0px 1px 8px #000015;
}
.fakeButtons {
  height: 10px;
  width: 10px;
  border-radius: 50%;
  border: 1px solid #000;
  position: relative;
  top: 0px;
  left: 10px;
  background-color: #ff3b47;
  border-color: #9d252b;
  display: inline-block;
}
.fakeMinimize {
  left: 15px;
  background-color: #ffc100;
  border-color: #9d802c;
}
.fakeZoom {
  left: 20px;
  background-color: #00d742;
  border-color: #049931;
}
.fakeMenu {
  width: 100%;
  box-sizing: border-box;
  height: 25px;
  background-color: #bbb;
  margin: 0 auto;
  border-top-right-radius: 5px;
  border-top-left-radius: 5px;
}
.fakeTerminal{
    padding: 2em 0 3em 3em;
    text-shadow: 0px 1px 5px #000015;
    background-color: #151515;
    box-sizing: border-box;
    border-radius: 0px 0px 5px 5px;
    opacity: 0.95;
}
.fakeTerminal h2{
    position: relative;
    font-size: 1.25em;
    white-space: nowrap;
    overflow: hidden;
    width: 0;
}
.line1 {
    color: #9CD9F0;
    -webkit-animation: type .5s 1s steps(20, end) forwards;
    -moz-animation: type .5s 1s steps(20, end) forwards;
    -o-animation: type .5s 1s steps(20, end) forwards;
    animation: type .5s 1s steps(20, end) forwards;
}
.cursor1 {
    -webkit-animation: blink 1s 2s 2 forwards;
    -moz-animation: blink 1s 2s 2 forwards;
    -o-animation: blink 1s 2s 2 forwards;
    animation: blink 1s 2s 2 forwards;
}
.line2 {
    color: #CDEE69;
    -webkit-animation: type .5s 4.25s steps(20, end) forwards;
    -moz-animation: type .5s 4.25s steps(20, end) forwards;
    -o-animation: type .5s 4.25s steps(20, end) forwards;
    animation: type .5s 4.25s steps(20, end) forwards;
}
.cursor2 {
    -webkit-animation: blink 1s 5.25s 2 forwards;
    -moz-animation: blink 1s 5.25s 2 forwards;
    -o-animation: blink 1s 5.25s 2 forwards;
    animation: blink 1s 5.25s 2 forwards;
}
.line3 {
    color: #E09690;
    -webkit-animation: type .5s 7.5s steps(20, end) forwards;
    -moz-animation: type .5s 7.5s steps(20, end) forwards;
    -o-animation: type .5s 7.5s steps(20, end) forwards;
    animation: type .5s 7.5s steps(20, end) forwards;
}
.cursor3 {
    -webkit-animation: blink 1s 8.5s 2 forwards;
    -moz-animation: blink 1s 8.5s 2 forwards;
    -o-animation: blink 1s 8.5s 2 forwards;
    animation: blink 1s 8.5s 2 forwards;
}
.line4 {
    color: #fff;
    -webkit-animation: type .5s 10.75s steps(20, end) forwards;
    -moz-animation: type .5s 10.75s steps(20, end) forwards;
    -o-animation: type .5s 10.75s steps(20, end) forwards;
    animation: type .5s 10.75s steps(20, end) forwards;
}
.cursor4 {
    -webkit-animation: blink 1s 11.5s infinite;
    -moz-animation: blink 1s 8.5s infinite;
    -o-animation: blink 1s 8.5s infinite;
    animation: blink 1s 8.5s infinite;
}

@-webkit-keyframes blink {
    0% {opacity: 0;}
    40% {opacity: 0;}
    50% {opacity: 1;}
    90% {opacity: 1;}
    100% {opacity: 0;}
}
@-moz-keyframes blink {
    0% {opacity: 0;}
    40% {opacity: 0;}
    50% {opacity: 1;}
    90% {opacity: 1;}
    100% {opacity: 0;}
}
@-o-keyframes blink {
    0% {opacity: 0;}
    40% {opacity: 0;}
    50% {opacity: 1;}
    90% {opacity: 1;}
    100% {opacity: 0;}
}
@keyframes blink {
    0% {opacity: 0;}
    40% {opacity: 0;}
    50% {opacity: 1;}
    90% {opacity: 1;}
    100% {opacity: 0;}
}
@-webkit-keyframes type { to {width: 100%;}}
@-moz-keyframes type { to {width: 100%;}}
@-o-keyframes type { to {width: 100%;}}
@keyframes type { to {width: 100%;}}

</style>
