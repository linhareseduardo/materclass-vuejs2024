<template>

    <div class="componente">

        <h1>Componente com Renderização Condicional</h1>
        <p>Nome: {{ nome }}</p>
        <p v-if="qtdCachorro === 0">Não tem Cachorro</p>
        <p v-else-if="qtdCachorro === 1">Tem um Cachorro</p>
        <p v-else>Tem muitos Cachorros</p>
    </div>

</template>

<script setup>

    import { defineProps } from 'vue';

    defineProps({
        nome: String,
        qtdCachorro: Number
    })


</script>