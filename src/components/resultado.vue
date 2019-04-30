<template>
    <div>
        <p>{{numero1}}</p>
        <p>{{numero2}}</p>
        <p>{{multiplicacao}}</p>
    </div>
</template>


<script>

export default {
    
    name: "resultado",

    props:{
        numero1:Number,
        numero2:Number
    },

    data: function(){
        return{
            soma: 0,
            multiplicacao:'',
            divisao:''
        }
    }
}

</script>