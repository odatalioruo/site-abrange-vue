<template>
<div class="tk">
    <div class="section">
        <b-row align-v="center" class="testando">
            <b-col cols md="2"></b-col>
            <b-col cols="10" md="5">
                <div class="sasas"></div>
                <div class="texto">
                        PEQUENOS REPAROS,<br> FAZEM A DIFERENÇA!
                </div>
            </b-col>
            <b-col cols="5"></b-col>
        </b-row>
    </div>
    <div class="test"></div>
</div>
</template>

<style lang="scss" scoped>
.tk{ overflow: hidden;}
.section {
  position:absolute;
  background: url('./img/banner1big.jpg');
  background-size: cover;
  color: black;
  clip-path: polygon(0% 100%, 0% 0%, 76% 0%, 100% 100%);
  height:75vh;
  width:70vw;
  z-index: 9999;
}
@media only screen and (max-width: 720px){
    .section{
        width:145vw;
    }
   .sasas{
    background:url('./img/obra1.png');
    background-size: contain;
    background-repeat: no-repeat;
    width:70%;
    height: 50px;
}
}

.test{
    background: url('./img/banner1small.jpg');
    background-size: cover;
    background-repeat: no-repeat;
    margin-left: 15vw;
    position:absolute;
    width:100%;
    height:100%;
    z-index: 10;
}
body {
  margin: 0;
  font: 20px/2.2 system-ui;
}
.testando{
    height: 70vh;
}
.sasas{
    background:url('./img/obra1.png');
    background-size: contain;
    background-repeat: no-repeat;

    width:120%;
    height: 80px;
}
.texto{
    padding-left:2em;
    font-size:1.2em;
    color: #456;
    font-style: italic;
}
</style>