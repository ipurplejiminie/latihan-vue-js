<script setup>
import { ref } from 'vue'
const count = ref(0)
const sukaKamu = () => count.value++
const kamu = () => count.value--
const pesan = (tulisan) => alert(tulisan)
const usia = (e) => {
  e.preventDefault()
  alert('benar')
}
</script>
<template>
  <h1>jumlah : {{ count }}</h1>
  <button @:click="sukaKamu">Like You</button>
  <button @:click="kamu">You</button>
  <button @click="pesan('contohnya')">lihat pesan</button><br />
  <form @:submit="usia">
    <input type="text" placeholder="masukin angka" />
    <input type="text" placeholder="masukin umur" />
    <button type="submit">submit</button>
  </form>
</template>
