<template>
    <div class="section">
        <b-row align-v="center" class="testando">
            <b-col cols="2"></b-col>
            <b-col cols="5">
                <div class="sasas"></div>
                <div class="texto">
                       A MÃO DE OBRA QUE FALTA,<br>NÓS TEMOS!
                </div>
            </b-col>
            <b-col cols="5"></b-col>
        </b-row>
    </div>
    <div class="test"></div>
</template>

<style lang="scss" scoped>

.section {
  position:absolute;
  background: url('./img/banner2big.jpg');
  background-size: cover;
  color: black;
  clip-path: polygon(0% 100%, 0% 0%, 76% 0%, 100% 100%);
  height:75vh;
  width:70vw;
  z-index: 9999;
}
.test{
    background: url('./img/banner2small.jpg');
    background-size: cover;
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
    background:url('./img/servico1.png');
    background-size: contain;
    background-repeat: no-repeat;

    width:120%;
    height: 80px;
}
.texto{
    padding-left:2em;
    font-size:1.3em;
    color: #456;
    font-style: italic;
}
</style>