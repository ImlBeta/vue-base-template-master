<template>
  <div>
      <a-textarea placeholder="Autosize height based on content lines" auto-size />
    <div style="margin: 24px 0" />
    <a-textarea
      placeholder="Autosize height with minimum and maximum number of lines"
      :auto-size="{ minRows: 2, maxRows: 6 }"
    />
    <div style="margin: 24px 0" />
    <a-textarea
      v-model="value"
      placeholder="Controlled autosize"
      :auto-size="{ minRows: 3, maxRows: 5 }"
    />
    <div class="components-input-demo-size">
    <a-input size="large" placeholder="large size" />
    <a-input placeholder="default size" />
    <a-input size="small" placeholder="small size" />
  </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      value: '',
      name: 'Ejemplo'
    };
  }
};
</script>
<style>
components-input-demo-size .ant-input {
  width: 200px;
  margin: 0 8px 8px 0;
}
</style>
