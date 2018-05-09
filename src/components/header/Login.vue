<template>
  <div id="LoginContainer">    

        <span>Acesse a plataforma</span> 
 
        <input class="form-control" type="text" placeholder="Login" />
    
        <input class="form-control" type="password" placeholder="Senha" />    
   
        <button type="button" class="btn">Entrar</button>
   
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
#LoginContainer {
  margin: 0;
  padding: 0 120px 0 0;
  background-color: #002b5b;
  min-height: 50px;
  display: flex;
  justify-content: flex-end;
  align-items: center;
}

#LoginContainer * {
  margin: 3px;
}

span {
  color: white;
  padding-right: 15px;
  font-weight: 600;
  font-size: 12px;
}

input {
  margin: 0 8px;
  width: 170px;
  height: 30px;
  border-radius: 7px;
}

button {
  background-color: #cd6701;
  color: white;
  border-radius: 7px;
}

@media (max-width: 640px) {
  #LoginContainer {
    flex-direction: column;
    justify-content: center;
    align-items: center;
    padding: 0;
  }
}
</style>
