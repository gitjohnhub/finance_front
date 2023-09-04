<template>
  <a-space direction="vertical">


    <a-card>

      <a-row>
        <a-col :span="12">
          <a-statistic title="Active Users" :value="112893" style="margin-right: 50px"
            :value-style="{ color: '#3f8600' }" />
        </a-col>
        <a-col :span="12">
          <a-statistic title="Account Balance (CNY)" :precision="2" :value="112893" />
        </a-col>
      </a-row>
    </a-card>

    <a-table :columns="columns" :data-source="data" :pagination="{ pageSize: 50 }"
      :scroll="{ y: 240 }" />

  </a-space>
</template>
<script lang="ts" setup>
const columns = [
  {
    title: 'Name',
    dataIndex: 'name',
    width: 150,
  },
  {
    title: 'Age',
    dataIndex: 'age',
    width: 150,
  },
  {
    title: 'Address',
    dataIndex: 'address',
  },
];

const data = [...Array(100)].map((_, i) => ({
  key: i,
  name: `Edward King ${i}`,
  age: 32,
  address: `London, Park Lane no. ${i}`,
}));
</script>

