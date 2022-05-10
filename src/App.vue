<template>
<div class="baba">
  <!-- <carousel /> -->
  <Menu />
  <carousel />
  <empresa />

  <onlin />
  <clientes />
  <servicos />  
  <cinza />
  <alimento />
  <verde />
  <controle />
  <roxo />
  <atend />


</div>

</template>

<script>
import cinza from './components/clientes cinza.vue'
import verde from './components/clientes verde.vue'
import roxo from './components/clientes roxo.vue'
import carousel from './components/carousel.vue'
import Menu from './components/menu.vue'
import Empresa from './components/empresa.vue'

import clientes from './components/clientes.vue'
import onlin from './components/onlin.vue'
import atend from './components/aten.vue'
import servicos from './components/servicos.vue'
import alimento from './components/alimentos.vue'
import controle from './components/controle.vue'

export default {
  name: 'App',
  components: {
    carousel,
    Menu,
    Empresa,
    clientes,
    onlin,
    atend,
    servicos,
    alimento,
    controle,
    cinza,
    verde,
    roxo
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

<style scoped>
.baba{
  overflow-x:hidden!important;
}
</style>