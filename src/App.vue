<template>
<div>
  <!-- <carousel /> -->
  <Menu />
  
  <carousel />
  <empresa />
  <gestao />
  <clientes />
  <onlin />
  <clientes />
  <servicos />  
  <clientes />
  <alimento />
  <clientes />
  <controle />
  <atend />
<slide4/>

</div>

</template>

<script>
import slide4 from './components/slide4.vue'
import carousel from './components/carousel.vue'
import Menu from './components/menu.vue'
import Empresa from './components/empresa.vue'
import gestao from './components/gestao.vue'
import clientes from './components/clientes.vue'
import onlin from './components/onlin.vue'
import atend from './components/aten.vue'
import servicos from './components/servicos.vue'

import alimento from './components/alimentos.vue'
import controle from './components/controle.vue'

export default {
  name: 'App',
  components: {
    slide4,
    carousel,
    Menu,
    Empresa,
    gestao,
    clientes,
    onlin,
    atend,
    servicos,
    alimento,
    controle
  }
}
</script>
<style >
body{ margin:0px; background: grey; background-size: 148%;

}

@font-face {
  font-family: 'regular';
  src: url('./components/font/Roboto-Regular.ttf');
}
@font-face {
  font-family: 'thin';
  src: url('./components/font/Roboto-Thin.ttf');
}
@font-face {
  font-family: 'Bold';
  src: url('./components/font/Roboto-Bold.ttf');
}
@font-face {
  font-family: 'Light';
  src: url('./components/font/Roboto-Light.ttf');
}
.laranja{
   color:rgb(255, 88,0); 
   font-family: 'Bold'!important;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  background-color:#fff;
}
html {
  scroll-behavior: smooth;
}
.center{
  display: flex;
  justify-content: center;
}
</style>