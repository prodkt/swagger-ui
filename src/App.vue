<template>
<div id="swagger-ui"></div>
</template>
<style scoped>
</style>
<script>
import { defineComponent } from "vue";

import SwaggerUI from "swagger-ui";

export default defineComponent({
  mounted() {
    SwaggerUI({
      dom_id: "#swagger-ui",
      openapi: "3.0.0",
      url: "https://petstore3.swagger.io/api/v3/openapi.json",
    });
  },
});
</script>