<script setup>
    import PrimeiroComponente from "./components/PrimeiroComponente.vue"
    import ComDados from "./components/ComDados.vue"
    import ComDadosReativosPrimitivos from "./components/ComDadosReativosPrimitivos.vue"
    import ComDadosReativosNaoPrimitivos from "./components/ComDadosReativosNaoPrimitivos.vue"
    import DataBinding from "./components/DataBinding.vue"
    import ComProps from "./components/ComProps.vue"
    import EscutaEvento from "./components/EscutaEvento.vue"

    const borracha = "borracha"
    const precoBorracha = 2.50
</script>

<template>
    <header> Vue </header>
    <EscutaEvento/>
    <ComProps :item="borracha" :preco="precoBorracha"/>
    <ComProps item="Lápis" v-bind:preco="0.50"/>
    <ComProps item="Apontador" v-bind:preco="1.50"/>
    <DataBinding/>
    <ComDadosReativosNaoPrimitivos/>
    <ComDadosReativosPrimitivos/>
    <ComDados/>
    <PrimeiroComponente/>
    <PrimeiroComponente/>
    <PrimeiroComponente/>
    <PrimeiroComponente/>
</template>

<style scoped>

</style>