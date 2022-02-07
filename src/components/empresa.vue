<template>
   <div>
        <div class="corpo">
                <h1 id="empresa" class="laranja">EMPRESA</h1>
            <p><span class="bold"> ABRANGE </span>, é um sistema para a gestão e controle de prestação de serviços<br>
            tecnológicos para o setor de construções civíl para obras públicas e privadas.<br>
            O ABRANGE oferece mais tecnologia, segurança de forma transparente de<br>
            relatórios e estatísticas para seus clientes.
            </p>
        </div>
   <h1 id="produtos" class="laranja">PRODUTOS</h1>
           

    <div class="container">     
        <div class="produtos">
            <div class="panel" v-for="(item, index) in produto" v-bind:key="index">
             <div>{{item.penis}}</div>
            </div>
        </div>
    </div>
        <h1 id="servicos" class="laranja">SERVIÇOS</h1>
   </div>
   

</template>



<script>

export default {
    
    data(){
        return{
       produto: [
           { id: 0, penis: 'acarro'},
           { id: 1, penis: 'banana'},
           { id: 2, penis: 'caqui'},
           { id: 3, penis: 'damasco'},
           { id: 4, penis: 'esmeralda'},
           
       ]
       }
    }
}
</script>

<style scoped>
#produtos{
  padding-bottom: 2em;
}
.container{ 
  color: white;
  padding: 1rem;
  padding-bottom: 3em;
}
.produtos{
  max-width: 1200px;
  margin: 0 auto;
  display: grid;
  grid-gap: 1rem;
  justify-content: center;
  max-width: 1024px;
}
@media (min-width: 700px){
    .produtos { grid-template-columns: repeat(3, 1fr); }
   
}
@media (max-width: 700px){
  .panel
 {
   background: linear-gradient(90deg, #789, #abc);
   min-height: 7em;
   min-width: 70vw;
   background-size: cover;
  
 }
}
.panel
 {
   background: linear-gradient(90deg, #789, #abc);
   min-height: 7em;
   background-size: cover;
  
 }
.laranja{font-size: 200%; margin-bottom: 0.3em;}
.bold{
    font-family: 'Bold';
    font-size: 1.5rem;
}
h1{
    font-size: 15pt;
    font-weight: 800;
    padding: 0px 10px 10px 10px;
    }
p{
        padding:2rem 5rem;
        color:#4a5a70;
        font-weight:600;
        line-height: 1.8;
        font-size:1.2em;
        font-family: 'Light';
        transform: scaleY(1.1);
       }
span{font-weight: 800;}

.corpo{
    min-height: 200px;
    max-height: 300px;
     padding:2.5rem;
     margin-bottom: 2rem;
     overflow:hidden;
         overflow: hidden;
    }

</style>