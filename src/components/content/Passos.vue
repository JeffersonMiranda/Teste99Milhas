<template>
  <div id="passosContainer">
      
      <h4>Como Funciona ?</h4>

      <div v-for="passo in conteudo" class="passosBox">
        <img :src="passo.imagem" height="150px"/>
        <div class="passosTextoContainer">        
          <h6>{{ passo.header }}</h6>
          <p>{{ passo.descricao }}</p>
        </div> 
      </div>

  </div>
</template>


<script>
import passosImage from "@/assets/passos/passos.png";

export default {
  data() {
    return {
      conteudo: [
        {
          header: "Passo a passo 1",
          imagem: passosImage,
          descricao:
            "Ao receber o bilhete você deverá conferir todos os dados da emissão. Caso haja algum erro com relação aos dados informados a Central Mibusca garante a correção sem nenhum custo adicional."
        },
        {
          header: "Passo a passo 2",
          imagem: passosImage,
          descricao:
            "Ao receber o bilhete você deverá conferir todos os dados da emissão. Caso haja algum erro com relação aos dados informados a Central Mibusca garante a correção sem nenhum custo adicional."
        },
        {
          header: "Passo a passo 3",
          imagem: passosImage,
          descricao:
            "Ao receber o bilhete você deverá conferir todos os dados da emissão. Caso haja algum erro com relação aos dados informados a Central Mibusca garante a correção sem nenhum custo adicional."
        }
      ]
    };
  }
};
</script>

<style lang="scss" scoped>
#passosContainer {
  width: 100%;
  height: auto;
  padding: 40px 120px;
  background-color: #dadada;
  display: flex;
  justify-content: center;
  flex-direction: column;
}

h4 {
  color: #909090;
  text-align: center;
  font-weight: bold;
  margin-bottom: 25px;
}

h4:before {
  content: "";
  display: block;
  background: url("/src/assets/Aviao Gray.png") no-repeat;
  width: 20px;
  height: 20px;
  float: left;
  margin: 0 6px 0 0;
}

.passosBox {
  max-width: 850px;
  display: flex;
  justify-content: center;
}

#passosContainer .passosBox:nth-child(3) {
  flex-flow: row-reverse;
  align-self: flex-end;
  text-align: right;
  .passosTextoContainer {
    padding-right: 15px;
    h6 {
      text-align: right;
    }
  }
}

.passosBox img {
  border: 3px solid #ce6e1d;
  border-radius: 7px;
}

.passosTextoContainer {
  display: flex;
  flex-flow: column;
  padding: 20px 0 0 15px;
}

.passosBox .passosTextoContainer h6 {
  color: #ce6e1d;
  font-weight: bold;
  text-align: left;
}

.passosBox .passosTextoContainer p {
  color: #585858;
}

@media (max-width: 640px) {
  .passosBox {
    flex-direction: column;
    align-items: center;
  }
  .passosBox .passosTextoContainer {
    align-items: center;
    text-align: center;
  }
  
#passosContainer .passosBox:nth-child(3) {
  flex-flow: column;
  align-self: center;
  text-align: center;
  .passosTextoContainer {
    padding-right: 15px;
    h6 {
      text-align: center;
    }
  }
}
}
</style>
