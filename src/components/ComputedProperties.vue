<script setup>
import { ref, computed } from 'vue'

const angka = ref(9)

const jumlahAngka = computed(() => {
  return angka.value * 5
})

const namaku = 'kyla'
const namaLain = 'dia'
const fullNama = computed(() => {
  return namaku + namaLain
})

const hitung = ref(0)
const hasilnya = computed(() => {
  return hitung.value * 5
})

const tempatHasil = () => {
  hitung.value++
}
</script>

<template>
  <h1>angka asli {{ angka }}</h1>
  <h1>angka kedua {{ jumlahAngka }}</h1>
  <h2>lengkap : {{ fullNama }}</h2>
  <h2>ngitung {{ hitung }}</h2>
  <h2>hasil {{ hasilnya }}</h2>
  <button @click="tempatHasil">Jumlah</button>
</template>
