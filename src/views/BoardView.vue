<template>
  <a-row>
    <a-col :span="12">
      <a-statistic title="Active Users" :value="112893" style="margin-right: 50px" />
    </a-col>
    <a-col :span="12">
      <a-statistic title="Account Balance (CNY)" :precision="2" :value="112893" />
    </a-col>
  </a-row>

  <a-row :gutter="[16,16]">
  <a-col :span="6">
    <CardView></CardView>
  </a-col>
  <a-col :span="6">
    <CardView></CardView>
  </a-col>
  <a-col :span="6">
    <CardView></CardView>
  </a-col>
  <a-col :span="6">
    <CardView></CardView>
  </a-col>
</a-row>
</template>
<script setup lang="ts">
import CardView from '@/components/CardView.vue';
</script>


