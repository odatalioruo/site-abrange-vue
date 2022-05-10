<template>
   <div>
        <div class="corpo">
            <h1 id="empresa" class="laranja">EMPRESA</h1>
              <b-row class="center">
                <b-col md="6">
                  <p><span class="bold"> 
                    ABRANGE </span>, é um sistema para a gestão e controle de prestação de serviços
                    tecnológicos para o setor de construções civíl para obras públicas e privadas.
                    O ABRANGE oferece mais tecnologia, segurança de forma transparente de
                    relatórios e estatísticas para seus clientes.
                  </p>
                </b-col>
              </b-row>
        </div>
   <h1 id="produtos" class="laranja">PRODUTOS</h1>
           

    <b-row class="contain">     
        <b-row ref="alpksd" class="produtos">
             <b-col cols="12" sm="2" class="panel" v-for="(item, index) in produto" v-bind:key="index">
              <div>
                <a  v-bind:href="item.link">
                <img class="sk" v-bind:src="item.emage" ><br>
                </a>
              </div>
            </b-col> 
             <!-- <li class="panel" v-for="(user,index) in users" v-bind:key="'user'+index">
               {{user.name}}<br>{{user.email}}<br>{{user.username}}<br>{{user.website}}
             </li> -->
        </b-row>
    </b-row>
        <h1 id="servicos" class="laranja">SERVIÇOS</h1>
   </div>
   

</template>



<script>
import axios from 'axios'
     

export default {
    methods: {
        Testeaxios(){
          const kk = this
          axios.get('https://jsonplaceholder.typicode.com/users')
          .then(function(response){
            console.log(response)
            kk.users = response.data
          })
        }

},
    // mixins: [baba],
    data(){
        return{
          users:[],
       produto: [
           { id: 0, emage: 'img/obras1.png', link: '#obras', nome: 'OBRAS'},
           { id: 1, emage: 'img/servico0.png', link: '#servico', nome: 'SERVIÇOS'},
           { id: 2, emage: 'img/alimentos1.png', link: '#alimentos', nome: 'ALIMENTOS'},
           { id: 3, emage: 'img/controle1.png', link: '#controle', nome: 'CONTROLE'},
       ],
       //peniano:[]
       }
    }
}
</script>

<style scoped>
#servicos{
  margin-top:1em;
  margin-bottom: 2em;
}
.sk{
  text-decoration: none;
  color: whitesmoke;
  font-weight: 700;
  font-family: 'light';
  letter-spacing: 1px;
height:100px; border-radius:1.3rem;
}
#produtos{
  padding-bottom: 2em;
}
.contain{ 
  color: white;
  padding: 1rem;
  padding-bottom: 3em;
}
.produtos{
  margin: 0 auto;
  justify-content: center;
  max-width: 1600px;
}
@media (min-width: 700px){
    .produtos { grid-template-columns: repeat(3, 1fr); }
   
}
@media (max-width: 700px){
  .sk{
  text-decoration: none;
  color: whitesmoke;
  font-weight: 700;
  font-family: 'light';
  letter-spacing: 1px;
height:100px; border-radius:1.3rem;
}
  .panel
 {
   /* background: linear-gradient(90deg, #789, #abc); */
   min-height: 7em;
   min-width: 70vw;
   margin: 4em;
   background-size: cover;

 }
}
.panel
 {
  display: flex;
  align-items: center;
  padding: 1em;
  margin: 1em;
  border-radius: 1.25em;
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
    }

@media only screen and (max-width: 1000px){
  p{ font-size:1.1em;}
   .corpo{
    min-height: 400px;
     padding:2.5rem;
     margin-bottom: 2rem;
     overflow:hidden;
    }

}
</style>