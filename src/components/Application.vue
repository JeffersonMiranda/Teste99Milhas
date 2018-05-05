<template>
  <div>
        <app-header></app-header>
        <app-content></app-content>
        <app-footer></app-footer>
  </div>
</template>


<script>
import AppHeader from "@/components/header/AppHeader.vue";
import AppContent from "@/components/content/AppContent.vue";
import AppFooter from "@/components/footer/AppFooter.vue";

export default {
  name: "Application",
  components: {
    AppHeader,
    AppContent,
    AppFooter
  }
};
</script>

<style scoped>

</style>
