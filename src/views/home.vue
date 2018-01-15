<script>
    import Destacados from "../components/Productos_destacados";
    import Programas from "../components/Programas";
    export default { 
        name: "Home",
        data(){
            return {
                datos:["Hola Mundo!!","JSlove","DigitalMind"]
            }
        },
        components:{Destacados,Programas},
    }   
</script>

<template>
    <div>
        <section>
            <Programas />
        </section>
        <section>
            <Destacados />
        </section>
    </div>
</template>

<style>
    
</style>
