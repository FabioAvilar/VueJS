<template>
    <h1>Meu nome é: {{nome}}</h1>
</template>

<script>
    export default {
        name: 'lyfeCycle',
        data() {
            return {
                nome: 'Ainda não sei'
            }
        },
        created() {
            setTimeout(() => {
                this.nome = 'Fabio'
            }, 1000);

            this.lifeCycle()
        },
        mounted() {
            setTimeout(() => {
                this.nome = 'Debora'
            }, 2000);

            this.lifeCycle()
        },
        methods: {
            lifeCycle() {
                console.log('Executou');
            }
        }
    }
</script>