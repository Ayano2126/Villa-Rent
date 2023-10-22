<template>
    <div class="login">
      <h2>Login</h2>
      <input v-model="username" placeholder="Username" />
      <input type="password" v-model="password" placeholder="Password" />
      <button @click="handleLogin">Login</button>
    </div>
</template>
  
<script>
  export default {
    data() {
      return {
        username: '',
        password: ''
      };
    },
    methods: {
      handleLogin() {
        if (this.username && this.password) {
          // 这里可以进行登录逻辑，例如发送请求到后端验证用户名和密码
          console.log('Logging in with', this.username, this.password);
        } else {
          alert('Please fill in both fields.');
        }
      }
    }
  };
</script>
  
  <style scoped>
  .login {
    /* 这里可以添加样式 */
  }
  </style>
  