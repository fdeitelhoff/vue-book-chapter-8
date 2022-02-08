<template>
  <div id="app">
    <Binding />
    <Rendering />
    <Form />
    <FormValidationManually />
  </div>
</template>

<script>
import Binding from './components/Binding.vue';
import Rendering from './components/Rendering.vue';
import Form from './components/Form.vue';
import FormValidationManually from './components/FormValidationManually.vue';

export default {
  name: 'App',
  components: {
    Binding,
    Rendering,
    Form,
    FormValidationManually,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  /* text-align: center; */
  color: #2c3e50;
  margin-top: 60px;
}
</style>
