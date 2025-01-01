<template>
    <div id="app">
      <div class="content">
        <h1>Halaman dengan Panah ke Bawah</h1>
        <p>Ini adalah contoh panah ke bawah di Vue.js.</p>
        <p>Scroll ke bawah dengan mengklik panah!</p>
        <!-- Konten tambahan untuk mensimulasikan halaman panjang -->
        <div style="height: 1200px;"></div>
      </div>
  
      <!-- Tombol Panah ke Bawah -->
      <div v-if="showArrow" class="down-arrow" @click="scrollToBottom">
        &#8595;
      </div>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        showArrow: true // Menampilkan panah ke bawah
      };
    },
    methods: {
      scrollToBottom() {
        // Scroll halaman ke bawah saat panah diklik
        window.scrollTo({
          top: document.documentElement.scrollHeight,
          behavior: "smooth" // Animasi smooth scrolling
        });
        this.showArrow = false; // Menyembunyikan panah setelah diklik
      }
    }
  };
  </script>
  
  <style scoped>
  #app {
    text-align: center;
    padding: 20px;
  }
  
  .content {
    padding: 20px;
  }
  
  .down-arrow {
    position: fixed;
    bottom: 20px;
    left: 50%;
    transform: translateX(-50%);
    font-size: 40px;
    cursor: pointer;
    color: #007BFF;
  }
  
  .down-arrow:hover {
    color: #0056b3;
  }
  
  h1, p {
    font-family: Arial, sans-serif;
  }
  </style>
  