<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <HelloWorld msg="Welcome to ImlBeta"/>
    <a-date-picker @change="onChange" />
    <a-upload>
           <a-button> <a-icon type="upload" /> Click to Upload </a-button>
    </a-upload>
    </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue';

export default {
  name: 'Home',
  components: {
    HelloWorld
  }
};
</script>
