<script setup lang="ts">
import NavView from './components/NavView.vue';
</script>

<template>
   <a-config-provider
    :theme="{
      token: {
        colorPrimary: '#ffd299',
      },
    }"
  >
  <NavView></NavView>
  </a-config-provider>

</template>

