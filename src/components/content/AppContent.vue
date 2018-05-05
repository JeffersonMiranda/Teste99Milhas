<template>
  <div id="AppContentContainer">
      
    <div id="banner">
    <img src="@/assets/banner.png">
    </div>

    <passos></passos>
    <depoimentos></depoimentos>
    <email-novidades></email-novidades>

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
  width: 100%;
}

#banner {
  width: 100%;
}

#banner img {
  width: 100%;
  border-top: 3px solid #cd6701;
}
</style>
