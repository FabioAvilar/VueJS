<template>
    <div>
        <img :src="avatar" :alt="descricao">
        <Reutilizacao />
    </div>
</template>

<script>
    import Reutilizacao from './reutilizacao.vue';
    export default {
    name: "picture",
    data() {
        return {
            avatar: "/img/SonicAdventure DC.jpeg",
            descricao: "O ouriço mais veloz dos games!"
        };
    },
    components: { 
        Reutilizacao 
    }
}
</script>