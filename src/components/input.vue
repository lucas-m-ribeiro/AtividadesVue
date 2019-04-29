<template>
    <div>
        <input  @input = "change" type="number" v-model="a">
        <input type="number" v-model="b">
        <p>{{a}}</p>
        <p>{{b}}</p>
    </div>
</template>

<script>

export default {
    name: "input1",
    data: function(){
        return {
            a: '',
            b: ''
        }
    },
    methods:{
        change(event){
            this.$emit('input_changed', event);
        },
    }
}

</script>

spring

gnirps
