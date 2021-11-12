<template>
  <div class="home">
    <!--<img alt="Vue logo" src="../assets/logo.png"> -->
    <img alt="Vue logo" src="../assets/Logo_CDMX.png">
    <img alt="Vue logo" src="../assets/Logo_Dependencia.png">
    <HelloWorld msg="Welcome to ImlBeta"/>
   <!-- <a-date-picker @change="onChange" />
    <a-upload>
           <a-button> <a-icon type="upload" /> Click to Upload </a-button>
    </a-upload> -->
    <a-form
    id="components-form-demo-normal-login"
    :form="form"
    class="login-form"
    @submit="handleSubmit"
  >
    <a-form-item>
      <a-input
        v-decorator="[
          'userName',
          { rules: [{ required: true, message: 'Please input your username!' }] },
        ]"
        placeholder="Username"
      >
        <a-icon slot="prefix" type="user" style="color: rgba(0,0,0,.25)" />
      </a-input>
    </a-form-item>
    <a-form-item>
      <a-input
        v-decorator="[
          'password',
          { rules: [{ required: true, message: 'Please input your Password!' }] },
        ]"
        type="password"
        placeholder="Password"
      >
        <a-icon slot="prefix" type="lock" style="color: rgba(0,0,0,.25)" />
      </a-input>
    </a-form-item>
    <a-form-item>
      <a-checkbox
        v-decorator="[
          'remember',
          {
            valuePropName: 'checked',
            initialValue: true,
          },
        ]"
      >
        Remember me
      </a-checkbox>
      <a class="login-form-forgot" href="">
        Forgot password
      </a>
      <a-button type="primary" html-type="submit" class="login-form-button">
        Log in
      </a-button>
      Or
      <a href="">
        register now!
      </a>
    </a-form-item>
  </a-form>

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

<style>

img {
  width: 250px;
  height: 75px ;
  margin: 2px;
  text-align: center;
  }

#components-form-demo-normal-login .login-form
{
  max-width: 300px;
}

#components-form-demo-normal-login .login-form-forgot
{
  float: right;
}
#components-form-demo-normal-login .login-form-button
{
  width: 100%;
}
</style>
