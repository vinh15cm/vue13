<template>
    <div>
      <div class="d-flex justify-space-between">
        <div style="width: 275px">
          <v-text-field
            v-model="search"
            label="Tìm kiếm"
            class="mr-2"
            density="compact"
            variant="outlined"
            append-icon="mdi-magnify"
          ></v-text-field>
        </div>
        <v-btn color="primary">Thêm mới</v-btn>
      </div>
  
      <div>
        <v-data-table
          v-model="selected"
          :items="items"
          item-value="name"
          show-select
        ></v-data-table>
      </div>
    </div>
  </template>
  <script setup>
  const selected = [];
  const items = [
    {
      name: "🍎 Apple",
      location: "Washington",
      height: "0.1",
      base: "0.07",
      volume: "0.0001",
    },
    {
      name: "🍌 Banana",
      location: "Ecuador",
      height: "0.2",
      base: "0.05",
      volume: "0.0002",
    },
    {
      name: "🍇 Grapes",
      location: "Italy",
      height: "0.02",
      base: "0.02",
      volume: "0.00001",
    },
    {
      name: "🍉 Watermelon",
      location: "China",
      height: "0.4",
      base: "0.3",
      volume: "0.03",
    },
    {
      name: "🍍 Pineapple",
      location: "Thailand",
      height: "0.3",
      base: "0.2",
      volume: "0.005",
    },
    {
      name: "🍒 Cherries",
      location: "Turkey",
      height: "0.02",
      base: "0.02",
      volume: "0.00001",
    },
    {
      name: "🥭 Mango",
      location: "India",
      height: "0.15",
      base: "0.1",
      volume: "0.0005",
    },
    {
      name: "🍓 Strawberry",
      location: "USA",
      height: "0.03",
      base: "0.03",
      volume: "0.00002",
    },
    {
      name: "🍑 Peach",
      location: "China",
      height: "0.09",
      base: "0.08",
      volume: "0.0004",
    },
    {
      name: "🥝 Kiwi",
      location: "New Zealand",
      height: "0.05",
      base: "0.05",
      volume: "0.0001",
    },
  ];
  </script>