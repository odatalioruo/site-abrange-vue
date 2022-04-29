<template>
        <div class="gestao">
        <div class="msg">
            <h1 style="display:flex; justify-content:center">GESTÃO PARA<br> CONSTRUÇÃO</h1>
            <span>VANTAGENS ABRANGE</span>
          <ul>
              <li>Aprovação de orçamentos de custos</li>
              <li>Agilidade na contratação de serviços</li>
              <li>Aluguel de máquinas pesadas e ferramentas</li>
              <li>Acesso à ampla rede credenciada de fornecedores</li>
              <li>Visualização em tempo real das demandas locais</li>
          </ul>
        </div>
    </div>
</template>




<script>
export default {
    
}
</script>


<style scoped>
h1{margin-left: .35em; font-family: 'Bold'; line-height: 1.1;margin-bottom:28px;}
span{margin:1.5em; font-family: 'Bold';}
.gestao{
    
   color:whitesmoke;
    min-height:640px;
    display:flex;
    background: url('./img/banner0.png');
    background-size: cover;
    align-items: center;
    font-family: 'Regular';
    }
    .msg{
    font-size: 1.5em;
    margin-left: 8vw;
    text-align: left;
    transform:scaleY(1.13)
 }
 ul{margin:0px;}
 li{font-size: .75em;}


 @media only screen and (max-width: 800px){
     .msg{
    font-size: 1.2em;
     margin-left: 0vw;
    padding: 0.5em;
    text-align: left;
    transform:scaleY(1.13)}
    .gestao{
            min-height:500px;
    }
 }
</style>