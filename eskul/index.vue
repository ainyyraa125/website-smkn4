<template>
  <section class="eskul-list">
    <div class="container">
      <h2>Ekstrakurikuler</h2>
      <div class="eskul-card" v-for="(eskul, index) in eskuls" :key="index">
        <img :src="eskul.image" :alt="eskul.name" />
        <h3>{{ eskul.name }}</h3>
        <p>{{ eskul.description }}</p>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'EskulList',
  data() {
    return {
      // Daftar ekstrakurikuler
      eskuls: [
        {
          name: 'IT CLUB',
          description: 'Bergabunglah dengan tim sepak bola untuk meningkatkan keterampilan bermain bola dan kerjasama tim.',
          image: '~/assets/img/ it club.jpeg'
        },
        {
          name: 'BASKET',
          description: 'Pelajari dan pertunjukkan tarian tradisional Indonesia yang penuh makna.',
          image: '~/assets/img/basket.jpeg'
        },
        {
          name: 'CJ',
          description: 'Latih kemampuan bermain basket dan jadilah bagian dari tim basket sekolah.',
          image: '~/assets/img/cj.jpeg'
        },
        {
          name: 'LASKAR',
          description: 'Latih kemampuan bermain basket dan jadilah bagian dari tim basket sekolah.',
          image: '~/assets/img/laskar.jpeg'
        },
        {
          name: 'PERISAI DIRI',
          description: 'Latih kemampuan bermain basket dan jadilah bagian dari tim basket sekolah.',
          image: '~/assets/img/perisai diri.jpeg'
        },
        {
          name: 'PKS',
          description: 'Latih kemampuan bermain basket dan jadilah bagian dari tim basket sekolah.',
          image: '~/assets/img/pks.jpeg'
        },
        {
          name: 'FUTSAL',
          description: 'Latih kemampuan bermain basket dan jadilah bagian dari tim basket sekolah.',
          image: '~/assets/img/futsal.jpeg'
        },
      ]
    }
  }
}
</script>

<style scoped>
.eskul-list {
  padding: 50px 0;
  background-color: #fff;
}

.eskul-list h2 {
  text-align: center;
  font-size: 2em;
  margin-bottom: 30px;
}

.eskul-card {
  background-color: #f9f9f9;
  border: 1px solid #ddd;
  border-radius: 5px;
  padding: 20px;
  margin-bottom: 20px;
  text-align: center;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
}

.eskul-card img {
  width: 100%;
  height: auto;
  border-radius: 5px;
}

.eskul-card h3 {
  font-size: 1.5em;
  margin: 10px 0;
}

.eskul-card p {
  font-size: 1em;
}
</style>
