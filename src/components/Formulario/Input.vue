<template>
<div>
  <label >Nombre</label>
  <input placeholder="Nombre" type="text"
   v-model="name"/>
        <input placeholder="Placa" type="text"
   v-model="placa"/>
  <a-textarea placeholder="Autosize height based on content lines" auto-size />
   <a-input-search placeholder="input search loading deault" loading />
</div>
</template>

<script>
export default {
  name: 'Input',
  data() {
    return {
      name: '',
      placa: ''
    };
  }
};
</script>

<style>
</style>
