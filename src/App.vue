<script setup lang="ts">
import NavView from './components/NavView.vue';
</script>

<template>
   <a-config-provider
    :theme="{
      token: {
        colorPrimary: '#00b96b',
      },
    }"
  >
  <NavView></NavView>
  </a-config-provider>

</template>

