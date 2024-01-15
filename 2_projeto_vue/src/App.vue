<template>
    <Header/>
    <ComponenteCerto />
    <LifeCycle />
    <Pessoa />
</template>

<script>
    import Header from './components/Header.vue';
    import ComponenteCerto from './components/ComponenteCerto.vue';
    import LifeCycle from './components/LifeCycle.vue';
    import Pessoa from './components/Pessoa.vue';
    export default {
        name: 'App',
        components: {
            ComponenteCerto,
            LifeCycle,
            Pessoa,
            Header,
        }
    }
</script>

<style>
    body{
        background-color: #333;
        color: #fff;
    }

    a{
        color: red;
    }

    .teste{
        background-color: black;
    }
</style>