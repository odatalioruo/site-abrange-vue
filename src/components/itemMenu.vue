<template>
    
    <div :class="(index % 2 === 0 ? 'par' : 'impar') + ' base'">
        <div :class="index % 2 === 0 ? 'tei' : 'tey'" ><p>{{text}}</p></div> 
    </div>
     <!-- <div :class="index % 2 === 0 ? 'tei' : 'tey'" ><p>{{text}}</p></div> -->

</template>
<script>
export default {
    name:'itemMenu',
    props: {
        text: String,
        index: Number
    },

}

</script>
<style scoped>
.par
{
    margin-top: 20px;
    height: 5em;
    width: 8em;
    background:#7ea1ae;
    transform: skewY(-10deg);
    transition-duration: .44s;
    position:relative;
}
.impar
{
    margin-top: 20px;
    height: 5em;
    width: 8em;
    background:#4a616e;
    transform: skewY(10deg);
    transition-duration: .44s;
     position:relative;
}
.tei
{
    background-image: linear-gradient( #fff0 50%,  #7ea1ae 50%);
    transform: skewY(10deg);
    padding: 2em 1em 2em 1em;
    transition-duration: .44s;    
}
.tey
{
    background-image: linear-gradient( #fff0 50%, #4a616e 50%);
    transform: skewY(-10deg);
    padding: 2em 1em 2em 1em;
    transition-duration: .44s;  
}
.par:hover
{
    transform: skewY(10deg);
}
.impar:hover
{
    transform: skewY(-10deg);
}
.tei:hover
{
    transform: skewY(-10deg);
}
.tey:hover
{
    transform: skewY(10deg);
}
</style>
