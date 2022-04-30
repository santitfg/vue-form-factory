<template>
  <h1>{{ msg }}</h1>
</template>

<script>
export default {
  name: "InputSelect",
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>

//  <div class="par">
//                 <label for="iProvincia">Provincia Institucion</label>
//                 <select
//                   id="iProvincia"
//                   v-model="dataInsti.provincia"
//                   name="iProvincia"
//                   @change="consultarDataGeoRef(dataInsti, 'departamentos')"
//                 >
//                   <option v-for="name in listaProv" :key="name">
//                     {{ name }}
//                   </option>
//                 </select>
//               </div>