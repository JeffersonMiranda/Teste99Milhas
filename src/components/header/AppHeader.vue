<template>
  <div id="AppHeaderContainer">
        <login></login>
        <nav-menu></nav-menu>
  </div>
</template>


<script>
import Login from "@/components/header/Login.vue";
import NavMenu from "@/components/header/NavMenu.vue";

export default {
  name: "AppHeader",
  components: {
    Login,
    NavMenu
  }
};
</script>

<style scoped>
#AppHeaderContainer {

}
</style>
