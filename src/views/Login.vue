<template>
  <section>
    <div class="login">
      <h1>Login</h1>
      <form>
        <label for="email">Email</label>
        <input type="email" name="email" id="email" v-model="login.email" />
        <label for="senha">Senha</label>
        <input type="password" name="senha" id="senha" v-model="login.senha" />
        <button class="btn" @click.prevent="logar">Logar</button>
      </form>
      <p class="reset-password">
        <a href="/" target="_blank">Perdeu a senha? Clique Aqui.</a>
      </p>
    </div>
    <LoginCriar />
  </section>
</template>

<script>
import LoginCriar from "@/components/LoginCriar";
export default {
  name: "login",
  components: { LoginCriar },
  data() {
    return {
      login: {
        email: "",
        senha: ""
      }
    };
  },
  methods: {
    logar() {}
  }
};
</script>

<style scoped>
h1 {
  text-align: center;
  font-size: 2rem;
  margin-top: 40px;
  color: #b9785f;
}
.login {
  max-width: 500px;
  margin: 0 auto;
  padding: 0 20px;
}
form {
  display: grid;
}
.btn {
  width: 100%;
  max-width: 300px;
  margin-left: auto;
  margin-right: auto;
}
.perdeu {
  text-align: center;
  margin: 20px auto 0 auto;
}
.perdeu a:hover {
  color: #87f;
  text-decoration: underline;
}
</style>
