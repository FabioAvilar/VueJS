<template>
    <div>
        <Reutilizacao />
        <h1>Ola Vue</h1>
        <p>Meu nome é {{nome}} e trabalho como {{profissao}}</p>
        <MultiplosEventos />
        <Reutilizacao />
        <Reutilizacao />
        <Reutilizacao />
    </div>
</template>

<script>
    import MultiplosEventos from './multiplosEventos.vue';
    import Reutilizacao from './reutilizacao.vue';
    export default {
    name: "PrimeiroComponente",
    data() {
        return {
            nome: "Fabio",
            profissao: "Programador"
        };
    },
    components: {
    MultiplosEventos,
    Reutilizacao
}
}
</script>