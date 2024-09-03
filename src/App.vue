<template>
  <div class="container">
    <div class="left-cont">
 <!--<h1>Bem-Vindo<br>Faça Login em nosso sistema</h1>-->
      <img src="/src/images/healthy-lifestyle-animate.svg" class="left-animation-image" alt="animação">
    </div>

    <div class="right-cont">
      <div class="card-login">
        <h1>Login</h1>
        <div class="textfield">
          <label for="usuario">Usuário</label>
          <input type="text" name="usuario" placeholder="Usuário">
        </div>

        <div class="textfield">
          <label for="senha">Senha</label>
          <input type="text" name="senha" placeholder="Senha">
        </div>
        <button class="btn-login">Realizar Login</button>
      </div>
    </div>

    
  </div>
</template>

<script setup>

</script>

<style scoped>

.container{
  width: 100vw;
  height: 100vh;
  background-color: #212121;
  display: flex;
  justify-content: center;
  align-items: center;
}

.left-cont{
  width: 50vw;
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}

.left-cont > h1{
  font-size: 3vw;
  color: #00ff88;
}

.right-cont{
  width: 50vw;
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
}

.left-animation-image{
  width: 75vh;
}

.card-login {
  width: 60%;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  padding: 30px 35px;
  background: #2f2841;
  border-radius: 20px;
  box-shadow: 0px 10px 40px #00000056;
}

.card-login > h1{
  color: #00ff88;
  font-weight: 900;
  margin: 0;
}

.textfield{
  width: 100%;
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  justify-content: center;
  margin: 10px 0px;
}

.textfield > input{
  width: 100%;
  border: none;
  border-radius: 10px;
  padding: 15px;
  background: #514864;
  color: #f0ffffde;
  font-size: 12pt;
  box-shadow: 0px 10px 40px #00000065;
  outline: none;
  box-sizing: border-box;
}

.textfield > label{
  color: #f0ffffde;
  margin-bottom: 10px;
  font-size: 20px;
}

.textfield > input::placeholder{
  color: #f0ffff94;
}

.btn-login{
  width: 100%;
  padding: 16px 0px;
  margin: 25px;
  border: none;
  border-radius: 10px;
  outline: none;
  text-transform: uppercase;
  font-weight: 800;
  color: #0b134b;
  background: #00ff88;
  cursor: pointer;
  box-shadow: 0px 10px 40px -12px #00ff8052;
}

@media only screen and (max-width: 950px){
  .card-login{
    width: 85%;
  }
}



@media only screen and(max-width: 600px){
  .container{
    flex-direction: column;
  }
  .left-cont > h1{
    display: none;
  }
}


</style>
