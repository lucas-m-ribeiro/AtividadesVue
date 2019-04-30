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
        evento(event){
            this.$emit('input', this.a, this.b);
        },
    }
}

</script>