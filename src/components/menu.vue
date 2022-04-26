<template>
    <div class="Menuu">
       <div> <img class="abrange" src="./img/abr.png"></div>
                    
            <ul class="caralho">
                <div class="he">  
                <!-- <li v-for="(item, index) in meni" v-bind:key="index" :class="index%2 === 0 ? 'par' : 'impar' "><a>{{item.funcao}}</a></li> -->
                <li v-for="(item, index) in meni" v-bind:key="index" >
                <a :href="item.href"><item-menu :text="item.funcao" :index="index" /> </a>
                </li>                
                <li Class="acesso" @click="penis()"><div class="tezi" ><a href="https://sistemagtf.com.br">ACESSO</a ></div></li>
                </div>
            </ul>    
                
        
    </div>
</template>
<script>
import itemMenu from './itemMenu.vue'


export default {
    el: '#o',
    name: 'menu',
    components: { itemMenu },
    data(){
        return{
       meni: [
           { id: 0, funcao:'EMPRESA', href: '#empresa'},
           { id: 1, funcao:'PRODUTOS', href: '#produtos'},
           { id: 2, funcao:'SERVIÇOS', href: '#servicos'},
           { id: 3, funcao:'PARCEIROS', href: '#parceiros'},
           { id: 4, funcao:'CONTATO', href: '#contato'},
           
       ],
       } 
    },
   
}
</script>
<!--Classes sempre declaradas em ordem de aparecimento-->
<style scoped>

.he{  width: 100%;
    height: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
    perspective: 100px;
}
.Menuu{
    display:none;
    
}
@media only screen and (min-width: 1024px){
    /* PC */
.Menuu{
    
    align-items: flex-end;
    display:flex;
    /* background: url('./img/tarja.png'); */
    background-image: linear-gradient(45deg, #49626f, #7fa1af);
    background-size: cover;
    height: 14vh;
    margin:0px;
         
}
.abrange{min-width: 21vw; margin-left:7.5vw; padding-right: 5vw; padding-bottom: 2vh; height: 8vh}
/* .impar{
    background-color:thistle;
}
.par{
    background-color: #78a;
} */
 ul.caralho {
     
    list-style-type: none;
    margin: 0;
    padding: 0;
    overflow: hidden;
    font-size: 10pt;
}

ul.caralho li {
    float: left;
    margin-left: 0.5vw;
    
}

ul.caralho li a {
    
    color: white;
    text-align: center;
    text-decoration: none;
}


ul.caralho li a.active {
    background-color:#04AA6D;
}
.acesso{
    margin-top: 20px;
    height: 5em;
    width: 8em;
     background: rgb(255, 88,0);
    transform: skewY(10deg);
    transition-duration: .7s;
     position:relative;
    
}
.tezi
{
    background-image: linear-gradient( #fff0 50%,  rgb(255, 88,0) 50%);
    transform: skewY(-10deg);
    padding: 25px;
    transition-duration: .7s;  
    margin:3px 0 3px 0;  
}
.acesso:hover{
     transform: skewY(-10deg);
}
.tezi:hover{
     transform: skewY(10deg);
}
/*

.itens{padding:1vw; margin:40px;}
.itens :hover{ background-color: aqua;}
*/
} 
</style>