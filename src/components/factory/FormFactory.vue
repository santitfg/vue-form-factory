
<script>
import InputText from "./InputText.vue";
import InputSelect from "./InputSelect.vue";

export default {
  name: "formFactory",
  props: {
    listJson: Object,
  },
  components: {
    InputText,
    InputSelect,
  },
  data() {
    return {
      comp: { InputSelect: "sdgd", InputText: "gdfgd" },

      componentes: { InputSelect: InputSelect, InputText: InputText },
      lista: [
        // InputText,
        "InputSelect",
        "InputText",
        null,
        "InputSelect",
        "fsdfa",
        "InputText",
      ],
      // listJson: [{ type: "InputText", msg: "esto es un test" }],
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
<template>
  <div v-for="(l, index) in listJson" :key="index">
    <!-- como hacer con el temilla de las keys -->
    <!-- https://es.vuejs.org/v2/guide/list.html -->
    <div v-if="l.type != null">
      <component :is="l.type" :msg="l.msg"> </component>
      <!-- <component :is="l" :msg="comp[l]"> </component> -->
      <!-- https://stackoverflow.com/questions/47155159/vue-js-how-to-get-key-left-side-value-from-json-property -->
      <!-- https://vuejs.org/guide/components/props.html#prop-passing-details -->
    </div>
  </div>
</template>