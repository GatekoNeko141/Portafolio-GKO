<template>
  <div class="snow">
    <div class="snowPanel snowPanel1">
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>		
    </div>
    <div class="snowPanel snowPanel2">
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>
    </div>
    <div class="snowPanel snowPanel3">
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>
      <i class="snowBall"></i>
    </div>
  </div>
</template>

<style scoped>
.snow{
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  overflow: hidden;
  z-index: 20;
  pointer-events: none;
}
.snowPanel{
  height: 200vh;
  margin-top: -200vh;
  position: relative;
  will-change: transform;
}
.snowBall{
  position: absolute;
  background: #fff;
  border-radius: 50%;
  box-shadow: #000 0px 1px 2px;
}
.snowBall:nth-child(1){
  left: 5%;
  top: 5%;
  width: 4px;
  height: 5px;
}
.snowBall:nth-child(2){
  left: 15%;
  top: 10%;
  width: 6px;
  height: 5px;
}
.snowBall:nth-child(3){
  left: 23%;
  top: 40%;
  width: 2px;
  height: 5px;
}
.snowBall:nth-child(4){
  left: 36%;
  top: 15%;
  width: 3px;
  height: 3px;
}
.snowBall:nth-child(5){
  left: 47%;
  top: 70%;
  width: 2px;
  height: 5px;
}
.snowBall:nth-child(6){
  left: 53%;
  top: 50%;
  width: 1px;
  height: 2px;
}
.snowBall:nth-child(7){
  left: 61%;
  top: 90%;
  width: 2px;
  height: 1px;
}
.snowBall:nth-child(8){
  left: 78%;
  top: 14%;
  width: 6px;
  height: 4px;
}
.snowBall:nth-child(9){
  left: 85%;
  top: 86%;
  width: 5px;
  height: 1px;
}
.snowBall:nth-child(10){
  left: 96%;
  top: 59%;
  width: 3px;
  height: 1px;
}
.snowBall:nth-child(11){
  left: 3%;
  top: 91%;
  width: 4px;
  height: 4px;
}
.snowBall:nth-child(12){
  left: 18%;
  top: 31%;
  width: 3px;
  height: 3px;
}
.snowBall:nth-child(13){
  left: 26%;
  top: 52%;
  width: 5px;
  height: 6px;
}
.snowBall:nth-child(14){
  left: 38%;
  top: 36%;
  width: 5px;
  height: 3px;
}
.snowBall:nth-child(15){
  left: 43%;
  top: 81%;
  width: 3px;
  height: 2px;
}
.snowBall:nth-child(16){
  left: 54%;
  top: 11%;
  width: 2px;
  height: 3px;
}
.snowBall:nth-child(17){
  left: 67%;
  top: 62%;
  width: 4px;
  height: 1px;
}
.snowBall:nth-child(18){
  left: 76%;
  top: 9%;
  width: 5px;
  height: 5px;
}
.snowBall:nth-child(19){
  left: 87%;
  top: 2%;
  width: 3px;
  height: 1px;
}
.snowBall:nth-child(20){
  left: 98%;
  top: 98%;
  width: 4px;
  height: 1px;
}
.snowBall:nth-child(21){
  left: 7%;
  top: 60%;
  width: 6px;
  height: 5px;
}
.snowBall:nth-child(22){
  left: 14%;
  top: 45%;
  width: 2px;
  height: 5px;
}
.snowBall:nth-child(23){
  left: 25%;
  top: 65%;
  width: 1px;
  height: 3px;
}
.snowBall:nth-child(24){
  left: 36%;
  top: 11%;
  width: 3px;
  height: 4px;
}
.snowBall:nth-child(25){
  left: 49%;
  top: 24%;
  width: 3px;
  height: 4px;
}
.snowBall:nth-child(26){
  left: 58%;
  top: 37%;
  width: 2px;
  height: 5px;
}
.snowBall:nth-child(27){
  left: 69%;
  top: 49%;
  width: 6px;
  height: 6px;
}
.snowBall:nth-child(28){
  left: 75%;
  top: 55%;
  width: 6px;
  height: 3px;
}
.snowBall:nth-child(29){
  left: 84%;
  top: 86%;
  width: 5px;
  height: 3px;
}
.snowBall:nth-child(30){
  left: 94%;
  top: 90%;
  width: 4px;
  height: 1px;
}
.snowBall:nth-child(31){
  left: 59%;
  top: 61%;
  width: 4px;
  height: 6px;
}
.snowPanel1{
  -webkit-animation: snow_1 8s linear infinite;
  animation: snow_1 8s linear infinite;
}
.snowPanel2{
  -webkit-animation: snow_2 13s 0s linear infinite;
  animation: snow_2 13s 0s linear infinite;
}
.snowPanel3{
  -webkit-animation: snow_3 16s 6s linear infinite;
  animation: snow_3 16s 6s linear infinite;
}
@-webkit-keyframes snow_1{
  0%{transform: translate(-250px, 0);}
  100%{transform: translate(250px, 300vh);}
}
@-webkit-keyframes snow_2{
  0%{transform: translate(0, 0);}
  100%{transform: translate(-100px, 300vh);}
}
@-webkit-keyframes snow_3{
  0%{transform: translate(-50px, 0);}
  100%{transform: translate(0, 300vh);}
}
@keyframes snow_1{
  0%{transform: translate(-250px, 0);}
  100%{transform: translate(250px, 300vh);}
}
@keyframes snow_2{
  0%{transform: translate(0, 0);}
  100%{transform: translate(-100px, 300vh);}
}
@keyframes snow_3{
  0%{transform: translate(-50px, 0);}
  100%{transform: translate(0, 300vh);}
}
</style>