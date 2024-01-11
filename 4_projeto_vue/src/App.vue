<template>
  <ComponenteCerto />
  <LifeCycle />
  <Pessoa />
</template>

<script>
  import ComponenteCerto from './components/ComponenteCerto.vue';
  import LifeCycle from './components/LifeCycle.vue';
  import Pessoa from './components/Pessoa.vue';

  export default {
      name: 'App',
      components: {
          ComponenteCerto,
          LifeCycle,
          Pessoa
      }
  }
</script>