<template>
    <div class="componente">
        <h1>Componente que Escuta Evento</h1>
        <p>Total: R${{ total }}</p>
        <div class="lista">
            <EmiteEvento item="Item1" :preco="1.99"/>
            <EmiteEvento item="Item2" :preco="5.00"/>
            <EmiteEvento item="Item3" :preco="10.99"/>
        </div>
    </div>
</template>

<script setup>

    import EmiteEvento from "./EmiteEvento.vue"

</script>

<style scoped>

    .lista{
        display: flex;
        justify-content: space-between;
    }

</style>