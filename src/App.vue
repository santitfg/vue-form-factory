<template>
  <img alt="Vue logo" src="./assets/logo.png" />
  <FormFactory :listJson="lista" />
</template>

<script>
import FormFactory from "./components/factory/FormFactory.vue";
export default {
  name: "App",
  components: {
    FormFactory,
  },
  data() {
    return {
      lista: [
        { type: "InputText", msg: "esto es un test" },
        { type: "InputSelect", msg: "esto es un select" },
      ],
    };
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
