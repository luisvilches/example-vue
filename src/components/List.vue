<script>
    export default { 
        name: "List",
        data(){
            return {
                title: "Home"
            }
        },
        props:["Lista"]
    }   
</script>

<template>
    <ul>
        <li v-for="item in Lista">{{item}}</li> 
    </ul>
</template>

<style>
    
</style>
