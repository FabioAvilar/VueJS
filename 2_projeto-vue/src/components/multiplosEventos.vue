<template>
    <div>
        <button @click="primeiro('Primeiro evento', $event), segundo($event), terceiro($event)">Ativar mútiplos eventos</button>
        <p>{{multiplos_eventos}}</p>
    </div>
</template>

<script>
    export default {
        name: 'MultiplosEventos',
        data() {
            return {
                multiplos_eventos: ""
            }
        },
        methods: {
            primeiro(txt, e) {
                 this.multiplos_eventos = txt
            },
            segundo(e) {
                setTimeout(() => this.multiplos_eventos = 'Segundo evento!', 500)
            },
            terceiro() {
                setTimeout(() => this.multiplos_eventos = '', 1500)
            }
        }
    }
</script>

<style scoped>
    div {
        margin: 100px;
    }
</style>