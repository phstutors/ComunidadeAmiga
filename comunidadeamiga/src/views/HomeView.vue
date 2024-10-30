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
          
          <a href="#" class="btn btn-link">Login</a>
        </div>
      </div>
      <div class="col-md-6 text-center">
        <img src="https://s3-alpha-sig.figma.com/img/5a17/67cc/520d83ae6950a8af0dec9c45f8b47983?Expires=1731283200&Key-Pair-Id=APKAQ4GOSFWCVNEHN3O4&Signature=WS~fpme~p~oLL~H19kpnLHb7Pb1~I02bq4VtQaKJ96bNYabFIAVyNm7RaNU6g-42SHFPziPoSz-Ceq95prdL5JTp0Jogt1IPyUHiXbFBzxHPpSx~tBLLQH5OPboEHOZ6NCYQSEcAZ9KuMeQ4MZ47oVs--Qy8to6txgRW07h1VrKB-S6rYJ8obJtivgtzKT3ORLUwdtEZMuF68Mj0lWjBfvsbEbFU6PAc9qE~ATv3~hzXMgYr~ZbCF9fXtXNEr7VS35IsajWBGmP6G2dgevpZZEzfQZMqcet7pOQI5gQ-qg2HpKzJJ1Ch4uQKBnosgc1YtWq8fQMVV7txRhaaP4q9OA__" alt="Imagem de Boas-vindas" class="img-fluid">
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
