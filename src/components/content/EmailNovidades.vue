<template>
  <div id="EmailNovidadesContainer">

    <h2> Informe seu e-mail e receba novidades </h2>

    <form>
      <input class="form-control" type="text" placeholder="Nome" />
      <input class="form-control" type="email" placeholder="E-mail" />    
      <button type="button" class="btn">Começar a Receber</button>  
    </form>

  </div>
</template>


<script>
export default {};
</script>


<style scoped>
#EmailNovidadesContainer {
  width: 100%;
  min-height: 200px;
  background-color: #002b5b;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-flow: column;
  flex-wrap: wrap;
}

h2 {
  color: white;
  text-align: center;
}

form {
  margin-top: 25px;
  display: flex;
  justify-content: center;
  align-items: center;
}

form input {
  margin: 0 18px;
  width: 350px;
  height: 30px;
}

form button {
  margin: 0 18px;
  padding: 0 5px;
  width: 160px;
  height: 30px;
  background-color: #cd6701;
  color: white;
  border-radius: 7px;
}

@media (max-width: 640px) {
  h2 {
    font-size: 18px;
  }
  form {
    width: 100%;
    flex-direction: column;
  }

  form input {
    width: 80%;
    margin: 4px;
  }
}
</style>
