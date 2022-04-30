<template>
  <div class="tab">
    <h1>{{ msg }}</h1>

    <input @change="null" />
  </div>
</template>

<script>
export default {
  name: "InputText",
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
