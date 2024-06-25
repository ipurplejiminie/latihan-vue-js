<script setup>
import { ref } from 'vue'
let tambahOrang = ref(['aku', 'kamu', 'dia'])
let dataOrang = ref({ nama: 'aku', umur: 20, tempat: ['bali', 'jawa'], nikah: false })
</script>

<template>
  <h1>Users List : {{ tambahOrang }}</h1>
  <button @click="tambahOrang.push('aku')">tambah lagi</button>
  <h2>nama : {{ dataOrang.nama }}</h2>
  <h2>umur : {{ dataOrang.umur }}</h2>
  <h2>tempat : {{ dataOrang.tempat }}</h2>
  <h2>nikah : {{ dataOrang.nikah }}</h2>
  <button @click="dataOrang.nama = 'mawar'">ganti nama</button>
  <button @click="dataOrang.umur = 50">ganti umur</button>
  <button @click="dataOrang.tempat = ['bumi', 'api']">ganti tempat</button>
  <button @click="dataOrang.nikah = 'true'">ganti nikah</button>
</template>
