<template>
    
    <div>
        <input type="number" v-model="a">
        <input type="number" v-model="b">
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