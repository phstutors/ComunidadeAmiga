<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
 
  <main>

    <section class="leftSide">
      <h1>Seja Bem Vindo ao ComunidadeAmiga</h1>
      <p>Ajude a criar uma comunidade mais unida e cheia de empatia, faça doações, crie seus eventos sociais e  
        faça seu pedido de doações..</p>

        <div class="buttonsContainer">
          <button href="" class="registerButton">Cadastre</button>
          <RouterLink to="/cadastro" class="loginButton">Login</RouterLink>
        </div>
    </section>

    <section class="rightSide">
        <img src="https://s3-alpha-sig.figma.com/img/5a17/67cc/520d83ae6950a8af0dec9c45f8b47983?Expires=1731283200&Key-Pair-Id=APKAQ4GOSFWCVNEHN3O4&Signature=WS~fpme~p~oLL~H19kpnLHb7Pb1~I02bq4VtQaKJ96bNYabFIAVyNm7RaNU6g-42SHFPziPoSz-Ceq95prdL5JTp0Jogt1IPyUHiXbFBzxHPpSx~tBLLQH5OPboEHOZ6NCYQSEcAZ9KuMeQ4MZ47oVs--Qy8to6txgRW07h1VrKB-S6rYJ8obJtivgtzKT3ORLUwdtEZMuF68Mj0lWjBfvsbEbFU6PAc9qE~ATv3~hzXMgYr~ZbCF9fXtXNEr7VS35IsajWBGmP6G2dgevpZZEzfQZMqcet7pOQI5gQ-qg2HpKzJJ1Ch4uQKBnosgc1YtWq8fQMVV7txRhaaP4q9OA__" alt="" srcset="">
    </section>

  </main>


</template>

<style scoped>

.registerButton{
  width: 159px!important;
  height: 50px;
  flex-shrink: 0;
  border: none;
  border-radius: 40px;
  background: #4DA3DF;
  box-shadow: -2px 22px 38px 0px #4DA3DF;
  color: #FFF;
  font-family: Poppins;
  font-size: 22px;
  font-style: normal;
  font-weight: 500;
  line-height: normal;
}
.leftSide p{
  color: #6B5E5E;
font-family: Inter;
font-size: 20px;
font-style: normal;
font-weight: 500;
line-height: normal;
}

.leftSide h1{ 
      color: #000;
    font-family: Inter;
    font-size: 58px;
    font-style: normal;
    font-weight: 700;
    line-height: 145.523%; 
}

main{
  display: flex;
  flex-direction: row;
  align-content: center;
  justify-content: center;
  align-items: center;
  flex-wrap: wrap;
}

.rightSide img{
  width: 820px;
}
.loginButton{
    color: #4D4D4D;
    font-family: Poppins;
    font-size: 22px;
    font-style: normal;
    font-weight: 600;
    line-height: normal;
    text-decoration: none;
    margin-left: 3%;
}

button:hover{
  cursor: pointer;
}
@media (max-width: 600px) {
  .rightSide img{
    width: 100%;
  }
  .leftSide{
    display: flex;
    flex-direction: column;
    align-content: center;
    align-items: center;
    justify-content: center;
  }
  .leftSide h1{
    font-size: 35px;
  }
}
.buttonsContainer{
  display: flex;
  flex-direction: row;
  align-content: center;
  align-items: center;
  justify-content: center;
}

</style>
