<script setup>
const pesan = 'aku lagi nyoba'
const angka = 400
function desimal(a, b) {
  return a - b
}
const prisma = 'https://www.prisma.io/'
const tulisan = 'aku lagi test aja'
</script>

<template>
  <h1>{{ angka }}</h1>
  <h2>Hasilnya adalah {{ desimal(8, 10) }}</h2>
  <h2>{{ pesan }}</h2>
  <a :href="prisma">ini link nya prisma</a>
  <p>{{ tulisan }}</p>
</template>
