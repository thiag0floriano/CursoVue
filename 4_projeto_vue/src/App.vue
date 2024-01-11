<template>
  <ComponenteCerto />
  <LifeCycle />
  <Pessoa />
  <Form />
</template>

<script>
  import ComponenteCerto from './components/ComponenteCerto.vue';
  import LifeCycle from './components/LifeCycle.vue';
  import Pessoa from './components/Pessoa.vue';
  import Form from './components/Form.vue';

  export default {
      name: 'App',
      components: {
          ComponenteCerto,
          LifeCycle,
          Pessoa,
          Form
      }
  }
</script>