<script setup>
import { ref, onMounted } from 'vue';
import { useScreen } from '@/composables/screen';
import axios from 'axios';

const { browserWidth, deviceWidth, isMobile } = useScreen();
const produtos = ref([]);

onMounted(async () => {
  const response = await axios.get('https://fakestoreapi.com/products');
  produtos.value = response.data;
});

const formatPrice = (price) => `R$ ${price.toFixed(2).replace('.', ',')}`;
</script>

<template>
  <div>
    <h1>
      <span v-if="isMobile">É móvel</span>
    </h1>
    <h1>Friends</h1>
    <div class="container">
      <div class="card">
        <h1 class="card--title">Livia</h1>
      </div>
      <div class="card">
        <h1 class="card--title">Brian</h1>
      </div>
      <div class="card">
        <h1 class="card--title">Rafael</h1>
      </div>
      <div class="card">
        <h1 class="card--title">Duda</h1>
      </div>
      <div class="card">
        <h1 class="card--title">Leandro</h1>
      </div>
      <div class="card">
        <h1 class="card--title">Maria</h1>
      </div>
      <div class="card">
        <h1 class="card--title">Isabelly</h1>
      </div>
      <div class="card">
        <h1 class="card--title">Lucas</h1>
      </div>
      <div class="card">
        <h1 class="card--title">Diego</h1>
      </div>
      <div class="card">
        <h1 class="card--title">Miguel</h1>
      </div>
    </div>
  </div>
</template>

<style scoped> @media (max-width: 768px) {
  .container {
    gap: 0.5rem;
  }
  .card {
    width: 92%;
  }
}

@media (min-width: 768px) and (max-width: 1024px) {
  .card {
    width: 22rem;
  }
}
.container {
  display: flex;
  flex-wrap: wrap;
  gap: 1rem;
  justify-content: center;
  align-items: center;
  margin: auto;
  padding: 1rem 0;
}
.card {
  display: flex;
  align-items: center;
  justify-content: space-between;
  flex-direction: column;
  width: 15rem;
  height: 25rem;
  background: #fff;
  box-shadow: 0 10px 20px rgba(0, 0, 0, 0.19), 0 6px 6px rgba(0, 0, 0, 0.23);
  border-radius: 10px;
  margin: auto;
  overflow: hidden;
}
.card--avatar {
  width: 100%;
  height: 17rem;
  object-fit: cover;
  margin-bottom: 0.5rem;
}
.card--title {
  color: #222;
  font-weight: 700;
  text-transform: capitalize;
  font-size: 1.1rem;
  margin-top: 0.5rem;
}
</style>