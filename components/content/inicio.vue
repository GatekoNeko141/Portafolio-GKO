<template>
    <b-container class="w-100">
        <h1>&lt;John Dev/&gt;</h1>
        <div class="pr-3">
            <div class=fakeMenu>
                <div class="fakeButtons fakeClose"></div>
                <div class="fakeButtons fakeMinimize"></div>
                <div class="fakeButtons fakeZoom"></div>
            </div>
            <div class="fakeTerminal">
                <h2 class="line1">¡Saludos! Bienvenido a mi portafolio web<span class="cursor1">_</span></h2>
                <h2 class="line2">Soy <strong>John Eymar Rodríguez Arteaga</strong><span class="cursor2">_</span></h2>
                <h2 class="line3">Programador FrontEnd.<span class="cursor3">_</span></h2>
                <h2 class="line4">$<span class="cursor4">_</span></h2>
            </div>
        </div>
    </b-container>
</template>

<style scoped>

.cont h1{
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
@media (max-width: 976px) {
    .cont h1{
        text-align: center;
        font-size: 35px;
        margin: 27vh 0 20px 0;
    }
    .fakeTerminal{
        padding-right: 10px !important;
    }
    .fakeTerminal h2{
        white-space: normal !important;
        width: 100% !important;
    }
    .cursor1, .cursor2, .cursor3{
        animation: none !important;
        opacity: 0;
    }
    .cursor4 {
        -webkit-animation: blink 1s 0.5s 2 infinite !important;
        -moz-animation: blink 1s 0.5s 2 infinite !important;
        -o-animation: blink 1s 0.5s 2 infinite !important;
        animation: blink 1s 0.5s 2 infinite !important;
    }
}
.fakeTerminal{
    padding: 2em 0 3em 3em;
    text-shadow: 0px 1px 5px #000015;
    background-color: rgb(21 21 21 / 85%);
    box-sizing: border-box;
    border-radius: 0px 0px 5px 5px;
    backdrop-filter: blur(5px);
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
