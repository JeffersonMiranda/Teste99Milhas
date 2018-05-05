<template>
  <div id="DepoimentosContainer">

      <h4>Depoimentos</h4> 
    
      <div id="depoimentosBoxes">
             
        <div v-for="depoimento in depoimentos" class="depoimentosBox">
            <img :src="depoimento.imagem" alt="">
            <h6>{{ depoimento.pessoa }}</h6>
            <span>{{ depoimento.cidade }}</span>
            <p>{{ depoimento.descricao }}</p>
        </div>

      </div>

  </div>
</template>


<script>
import JoseAlmeidaImg from "@/assets/depoimentos/jose_almeida.png";
import PaulaAndradeImg from "@/assets/depoimentos/paula_andrade.png";

export default {
  data() {
    return {
      depoimentos: [
        {
          pessoa: "José Almeida",
          cidade: "Imperatriz",
          imagem: JoseAlmeidaImg,
          descricao:
            '"A Mibusca é uma empresa que passa segurança, pois além de ter um serviço muito útil, possui profissionais excelentes e atendimento eficiente. Tenho certeza que a partir de agora vou fazer sempre a melhor escolhanas viagens que preciso fazer."'
        },
        {
          pessoa: "Paula Andrade",
          cidade: "Imperatriz",
          imagem: PaulaAndradeImg,
          descricao:
            '"A Mibusca é uma empresa que passa segurança, pois além de ter um serviço muito útil, possui profissionais excelentes e atendimento eficiente. Tenho certeza que a partir de agora vou fazer sempre a melhor escolhanas viagens que preciso fazer."'
        },
        {
          pessoa: "José Almeida",
          cidade: "Imperatriz",
          imagem: JoseAlmeidaImg,
          descricao:
            '"A Mibusca é uma empresa que passa segurança, pois além de ter um serviço muito útil, possui profissionais excelentes e atendimento eficiente. Tenho certeza que a partir de agora vou fazer sempre a melhor escolhanas viagens que preciso fazer."'
        }
      ]
    };
  }
};
</script>


<style scoped>
#DepoimentosContainer {
  width: 100%;
  height: 500px;
  background-color: #ffffff;
  display: flex;
  flex-flow: column;
  justify-content: center;
  align-items: center;
}

h4 {
  color: #909090;
  text-align: center;
  padding-bottom: 20px;
  font-weight: bold;
}

#depoimentosBoxes {
  display: flex;
  justify-content: center;
}

.depoimentosBox {
  display: flex;
  align-items: center;
  flex-direction: column;
  max-width: 400px;
  padding: 0 15px;
}

.depoimentosBox h6 {
  color: #012c5b;
  font-weight: bold;
  padding-top: 10px;
}

.depoimentosBox span {
  color: #cd6702;
  font-weight: bold;
  font-size: 12px;
}

.depoimentosBox p {
  text-align: center;
  color: #606060;
}


</style>
