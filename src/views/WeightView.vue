<template>
  <a-space direction="vertical">

  <FormView />

  <a-segmented v-model:value="value" :options="data" />
</a-space>

</template>
<script lang="ts" setup>
import { reactive, ref } from 'vue';
import FormView from '@/components/Weight/FormView.vue';
const data = reactive(['Daily', 'Weekly', 'Monthly', 'Quarterly', 'Yearly']);
const value = ref(data[0]);
</script>

