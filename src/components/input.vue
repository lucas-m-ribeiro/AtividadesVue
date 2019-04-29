<template>
    <div>
        <input type="number" v-model="a">
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
    }
}
</script>
