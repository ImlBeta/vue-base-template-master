<template>
  <nav class="app-navbar">
    <a-row>
      <NavButton label="Login" path="/" :grid="gridButtons" />
      <NavButton label="About" path="/about" :grid="gridButtons" />
      <NavButton label="Info" path="/mau" :grid="gridButtons" />
      <NavButton label="Boton" path="/ejemplo" :grid="gridButtons" />
    </a-row>
  </nav>
</template>
<script>
import NavButton from '@/components/Navbar/NavButton.vue';

export default {
  name: 'Navbar',
  components: {
    NavButton
  },
  data() {
    return {
      gridButtons: {
        xs: 24,
        sm: 24,
        md: 24,
        lg: 6,
        xl: 4,
        xxl: 4
      }
    };
  }
};
</script>

<style>
.app-navbar{
  background: rgb(159, 34, 65);
}
.nav-button{
  background-color: rgb(159, 34, 65);
  min-height: 35px;
  display: flex;
  justify-content: center;
  align-items: center;
  font-size: 20px;
  color: white;
  font-weight: bold;
}
.nav-button:hover{
  background-color: rgb(245, 183, 67);
  cursor: pointer;
}
</style>
