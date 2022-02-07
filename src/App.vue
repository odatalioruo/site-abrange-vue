<template>
<div>
  <Menu />
  <Card />
  <empresa />
  <gestao />
  <clientes />
  <onlin />
  <atend />
</div>

</template>

<script>
import Menu from './components/menu.vue'
import Card from './components/card.vue'
import Empresa from './components/empresa.vue'
import gestao from './components/gestao.vue'
import clientes from './components/clientes.vue'
import onlin from './components/onlin.vue'
import atend from './components/aten.vue'
export default {
  name: 'App',
  components: {
    Menu,
    Card,
    Empresa,
    gestao,
    clientes,
    onlin,
    atend
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
</style>