<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>
<template>
  <div class="container my-5">
    <div class="row align-items-center">
      <div class="col-md-6 text-center text-md-left">
        <h1 class="display-4 font-weight-bold">Seja Bem Vindo ao<br>ComunidadeAmiga</h1>
        <p class="lead">
          Ajude a criar uma comunidade mais unida e cheia de empatia, faça doações, crie seus eventos sociais e
          faça seu pedido de doações..
        </p>
        <div class="mt-4">

          <RouterLink to="/cadastro" class="btn btn-primary btn-lg mr-3">Cadastre-se</RouterLink>
          <RouterLink to="/login" class="btn btn-link">Login</RouterLink>
        </div>
      </div>
      <div class="col-md-6 text-center">
        <img src="https://i.imgur.com/lIzcNcs.png" alt="Imagem de Boas-vindas" class="img-fluid">
        <div class="mt-3">
          <span class="badge badge-danger p-2">Visite o Comunidade Amiga</span>
        </div>
      </div>
    </div>
  </div>

    <Footer/>
</template>

<style scoped>
.footer {
  background-color: #f5f5f5;
  padding: 20px;
}

.social-icons i {
  color: #6c757d;
  transition: color 0.3s;
}

.social-icons i:hover {
  color: #007bff;
}
</style>


<script>
import NavBar from '../components/NavBar.vue';
import Footer from '../components/Footer.vue';

export default {
  components: {
    NavBar,
    Footer,
  },
};
</script>
