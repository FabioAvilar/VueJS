<template>
    <div>
        <h2>Esta é a descrição da pessoa: {{nome}}</h2>
        <info :email='email' :esta_trabalhando=true />
    </div>
</template>

<script>
    import info from './info.vue'

    export default {
        name: 'Pessoa',
        components: { 
            info 
        },
        data() {
            return {
                nome: 'Matheus',
                email: 'fabio@email.com'
            }
        }
    }
</script>