<template>
  <div id="AppFooterContainer">
      
    <div id="LogoBox">
      <hr>
      <img src="@/assets/MibuscaLogoRodape.png">
      <hr>
    </div>   
  
   <div id="FooterBoxes">

    <div id="AtendimentoContainer">
      <ul>
        <li>ATENDIMENTO: 0300 313 5568</li>
        <li>MIBUSCA VIAGENS E TURISMO</li>
        <li>CNPJ: 99.999.999/0001-99</li>
        <li> 
          <img src="@/assets/footer/redes_sociais/Facebook.png">
          <img src="@/assets/footer/redes_sociais/Instagram.png">
        </li>
      </ul>
    </div>

    <div id="MenuContainer">
       <ul>
        <li><a href="#">Quem somos</a></li>
        <li><a href="#">Cadastra - se</a></li>
        <li><a href="#">Política de Privacidade</a></li>
        <li><a href="#">Termos e Condições</a></li>
       </ul>
    </div>

    <div id="PagamentosContainer">
        <h5>Pagamento</h5>
        <ul id="listaCartoes">
          <li><img src="@/assets/footer/cartoes/Visa.png" width="65" height="35"></li>
          <li><img src="@/assets/footer/cartoes/Mastercard.png" width="65" height="35"></li>
          <li><img src="@/assets/footer/cartoes/Elo.png" width="65" height="35"></li>
          <li><img src="@/assets/footer/cartoes/Diners Club.png" width="65" height="35"></li>
          <li><img src="@/assets/footer/cartoes/American Express.png" width="65" height="35"></li>
          <li><img src="@/assets/footer/cartoes/Hipercard.png" width="65" height="35"></li>
        </ul>
    </div>

    <div id="CertificadosContainer">
       <h5>Certificados</h5>
       <ul>
        <li><img src="@/assets/footer/certificados/Site Blindado.png"></li>
        <li><img src="@/assets/footer/certificados/McAfee Secure.png"></li>
       </ul>
    </div>

    </div>

  </div>
</template>


<script>
export default {};
</script>


<style scoped>
#AppFooterContainer {
  padding: 20px 0;
  background-color: #d2d2d2;
  color: #7f7f7f;
}

#LogoBox {
  display: flex;
  align-items: center;
  padding: 15px 0;
}

#LogoBox img {
  margin: 0;
  padding: 0 10px;
}

#LogoBox hr {
  width: 100%;
  padding: 0;
  margin: 0;
  border: 2px solid #cd6701;
}

#LogoBox hr:nth-child(1) {
  width: 130px;
}

ul {
  padding: 0;
  margin: 0;
  list-style: none;
}

ul li a {
  color: #7f7f7f;
  text-decoration: none;
}

#FooterBoxes {
  display: flex;
  justify-content: space-between;
  padding: 0 90px;
}

/*
#FooterBoxes div:nth-child(2), #FooterBoxes div:nth-child(3), #FooterBoxes div:nth-child(4) {
  border-left: 1px solid gray; 
}
*/

#PagamentosContainer ul {
  display: flex;
  flex-wrap: wrap;
  justify-content: flex-start;
  width: 250px;
}

#PagamentosContainer ul li {
  padding: 2px 10px 0 0;
}

#PagamentosContainer ul li img {
  margin: 0;
  padding: 0;
}

#CertificadosContainer ul li {
  padding: 0 0 5px 0;
}

@media (max-width: 640px) {
  #LogoBox {
    justify-content: center;
  }
  #FooterBoxes {
    flex-direction: column;
    justify-content: space-between;
    align-items: center;
    padding: 0 90px;
    text-align: center;
  }

  #FooterBoxes > div{
    margin:5px 0;
  }

  #LogoBox hr {
    width: 50%;
    padding: 0;
    margin: 0;
    border: 2px solid #cd6701;
  }

  #LogoBox hr:nth-child(1) {
    width: 50%;
  }

  #PagamentosContainer ul {
    justify-content: center;
  }
}
</style>
