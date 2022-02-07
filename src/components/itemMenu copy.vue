<template>

    <div :class="(index % 2 === 0 ? 'par' : 'impar') + ' base'">
        <!-- <div :class="index % 2 === 0 ? 'tei' : 'tey'" ><p>{{text}}</p></div> -->
        <div class="ostexto"><p>{{text}}</p></div>
        <div :class="'animado'"></div>
    </div>

</template>
<script>
export default {
    name:'itemMenu',
    props: {
        text: String,
        index: Number
    }
}
</script>
<style scoped>
.base {
    position: relative
}
.ostexto {
    width: 100%;
    margin: auto;
    z-index: 20;  
    position: absolute;
}

.par>.animado
{
    /* position: ; */
    width: 100%;
    min-width: 100px;
    height: 50px;
    margin: 0px;
    background: rgb(116, 141, 164);
    transition: 0.3s;
    z-index: 0;         
}



.impar>.animado
{
    /* position: absolute; */
    width: 100%;
    min-width: 100px;
    height: 50px;
    margin: 0px;
    background: rgb(54, 77, 90);
    transition: 0.3s;
}

.stage1 {
    transform: skewY(-10deg); 
}
.stage2 {
    transform: skewY(10deg); 
}
</style>
