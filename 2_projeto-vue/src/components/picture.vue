<template>
    <div>
        <img :src="avatar" :alt="descricao">
    </div>
</template>

<script>
    export default {
        name: 'picture',
        data() {
            return {
                avatar: "/img/SonicAdventure DC.jpeg",
                descricao: "O ouriço mais veloz dos games!"
            }
        }
    }
</script>