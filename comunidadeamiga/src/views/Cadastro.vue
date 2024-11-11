<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>
<template>
  <div class="container my-5 align-items-center">
    <div class="row align-items-center">
      <div class="col-md-6 text-center leftSide" style="background-color: #9DCCED; height: 100%;">
        <img src="https://i.imgur.com/lIzcNcs.png" alt="Imagem de Boas-vindas" class="img-fluid">
        <div class="mt-3">
          <h1 class="text-white">ComunidadeAmiga</h1>
          <span class="badge badge-danger p-2">Faça sua doação e crie um mundo melhor,
            cheio de soledariedade e empatia.</span>
        </div>
      </div>
      <div class="col-md-6 text-center text-md-left">
        <img src="https://s3-alpha-sig.figma.com/img/5a17/67cc/520d83ae6950a8af0dec9c45f8b47983?Expires=1731283200&Key-Pair-Id=APKAQ4GOSFWCVNEHN3O4&Signature=WS~fpme~p~oLL~H19kpnLHb7Pb1~I02bq4VtQaKJ96bNYabFIAVyNm7RaNU6g-42SHFPziPoSz-Ceq95prdL5JTp0Jogt1IPyUHiXbFBzxHPpSx~tBLLQH5OPboEHOZ6NCYQSEcAZ9KuMeQ4MZ47oVs--Qy8to6txgRW07h1VrKB-S6rYJ8obJtivgtzKT3ORLUwdtEZMuF68Mj0lWjBfvsbEbFU6PAc9qE~ATv3~hzXMgYr~ZbCF9fXtXNEr7VS35IsajWBGmP6G2dgevpZZEzfQZMqcet7pOQI5gQ-qg2HpKzJJ1Ch4uQKBnosgc1YtWq8fQMVV7txRhaaP4q9OA__" alt="Imagem de Boas-vindas" class="img w-25">
        <h1 class="display-4 font-weight-bold">Cadastre sua conta</h1>
        <span class="text-secondary">Faça sua doação e crie um mundo melhor</span>
        <p class="text-white m-2 p-1 rounded" style="background-color: #FF0000;">Cadastre-se com o google</p>
        <p class="text-muted">Ou cadastrar com email</p>
        <div class="mt-4">
          <div class="input-group input-group-sm mb-3">
                <div class="input-group-prepend">
                  <span class="input-group-text" id="inputGroup-sizing-sm">Nome</span>
                </div>
                <input type="text" class="form-control" aria-label="Small" placeholder="Digite seu nome" aria-describedby="inputGroup-sizing-sm">
          </div>
            <div class="input-group input-group-sm mb-3">
                      <div class="input-group-prepend">
                        <span class="input-group-text" id="inputGroup-sizing-sm">Email</span>
                      </div>
                      <input type="email" class="form-control" aria-label="Small" placeholder="Digite seu nome" aria-describedby="inputGroup-sizing-sm">
            </div>
            <div class="input-group input-group-sm mb-3">
                      <div class="input-group-prepend">
                        <span class="input-group-text" id="inputGroup-sizing-sm">Senha</span>
                      </div>
                      <input  :type="inputType" v-model="password"   class="form-control" aria-label="Small" placeholder="Digite seu nome" aria-describedby="inputGroup-sizing-sm">
            </div>
            <div class="input-group mb-3">
                <div class="input-group-prepend">
                  <span class="input-group-text">Foto de Perfil</span>
                </div>
                <div class="custom-file">
                  <input type="file" class="custom-file-input" id="inputGroupFile01">
                </div>

                <div class="input-group mt-3">
                <div class="input-group-prepend">
                  <div class="input-group-text">
                    <input type="checkbox" aria-label="Checkbox for following text input"  v-model="isVisibility"/>
                  </div>
                </div>
                <span class="text-secondary">Mostrar senha</span>
              </div>

              <div class="d-flex justify-content-center w-100">
                <button type="button" class="btn btn-success w-50 m-2" style="background-color: #31D009; border: none;">Cadastrar</button>
              </div>
              <div class="d-flex justify-content-center w-100">
                <span class="text-secondary">Tem conta? <router-link to="/login" class="text-secondary">Volte para tela de login agora!</router-link></span>
              </div>
            </div>
         
        </div>
      </div>
      
    </div>
  </div>
</template>

<style scoped>

.fill{
  height: 100vh!important;
}
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
@media (max-width: 600px) {
  .leftSide {
    display: none;
  }
}
</style>

<script>

export default{
  data () {
    return {
        password: '',
        isVisibility: false
    }
  },
  computed: {

    inputType(){

        return this.isVisibility ? 'text' : 'password';

    }
  },
};
</script>
