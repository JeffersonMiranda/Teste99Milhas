<template>
  <div id="AppContentContainer">
    <!--
    <div id="banner">
    <img src="@/assets/banner.png">
    </div> 
    -->
    <passos></passos> <!-- ID=passosContainer -->
    <depoimentos></depoimentos> <!-- ID=DepoimentosContainer -->
    <email-novidades></email-novidades> <!-- ID=EmailNovidadesContainer -->
  </div>
</template>


<script>
import Passos from "@/components/content/Passos.vue";
import Depoimentos from "@/components/content/Depoimentos.vue";
import EmailNovidades from "@/components/content/EmailNovidades.vue";

export default {
  name: "AppContent",
  components: {
    Depoimentos,
    Passos,
    EmailNovidades
  }
};
</script>

<style scoped>
#AppContentContainer {
  display: grid;
  grid-template-columns: 1fr;
  grid-template-rows: auto auto auto auto;
  grid-template-areas:
    "banner"
    "passos"
    "depoimentos"
    "email_novidades";
}

#banner {
  grid-area: banner;
}

#passos {
  grid-area: passos;
}

#depoimentos {
  grid-area: depoimentos;
}

#email_novidades {
  grid-area: email_novidades;
}

#banner img {
  border-top: 3px solid #cd6701;
  width: 100%;
  height: auto;
}
</style>
