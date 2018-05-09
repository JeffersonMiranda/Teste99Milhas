<template>
  <div class="grid">
        <app-header class="app_header"></app-header>
     
        <app-content class="app_content"></app-content>
       
        <app-footer class="app_footer"></app-footer>
       
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
html,
body {
  width: 100%;
  height: 100%;
}

.grid {
  height: 100%;
  display: grid;
  grid-template-columns: 1fr;
  grid-template-rows: auto auto auto;
  grid-template-areas:
    "header"
    "content"
    "footer";
}

.app_header {
  grid-area: header;
}

.app_content {
  grid-area: content;
}

.app_footer {
  grid-area: footer;
}
</style>
