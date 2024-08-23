<script setup>
import { useScreen } from '@/composables/screen';

const { isMobile } = useScreen();

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
        <li class="topic">Data de Aniversário:</li>
        <li class="topic">Cor Favorita:</li>
        <li class="topic">Comida Favorita:</li>
        <li class="topic">Bebida Favorita:</li>
        <li class="topic">Filme Favorito:</li>
        <li class="topic">Desenho Favorito:</li>
        <li class="topic">Banda/Cantor(a):</li>
      </div>
      <div class="card">
        <h1 class="card--title">Brian</h1>
        <li class="topic">Data de Aniversário:</li>
        <li class="topic">Cor Favorita:</li>
        <li class="topic">Comida Favorita:</li>
        <li class="topic">Bebida Favorita:</li>
        <li class="topic">Filme Favorito:</li>
        <li class="topic">Desenho Favorito:</li>
        <li class="topic">Banda/Cantor(a):</li>
      </div>
      <div class="card">
        <h1 class="card--title">Rafael</h1>
        <li class="topic">Data de Aniversário:</li>
        <li class="topic">Cor Favorita:</li>
        <li class="topic">Comida Favorita:</li>
        <li class="topic">Bebida Favorita:</li>
        <li class="topic">Filme Favorito:</li>
        <li class="topic">Desenho Favorito:</li>
        <li class="topic">Banda/Cantor(a):</li>
      </div>
      <div class="card">
        <h1 class="card--title">Duda</h1>
        <li class="topic">Data de Aniversário:</li>
        <li class="topic">Cor Favorita:</li>
        <li class="topic">Comida Favorita:</li>
        <li class="topic">Bebida Favorita:</li>
        <li class="topic">Filme Favorito:</li>
        <li class="topic">Desenho Favorito:</li>
        <li class="topic">Banda/Cantor(a):</li>
      </div>
      <div class="card">
        <h1 class="card--title">Leandro</h1>
        <li class="topic">Data de Aniversário:</li>
        <li class="topic">Cor Favorita:</li>
        <li class="topic">Comida Favorita:</li>
        <li class="topic">Bebida Favorita:</li>
        <li class="topic">Filme Favorito:</li>
        <li class="topic">Desenho Favorito:</li>
        <li class="topic">Banda/Cantor(a):</li>
      </div>
      <div class="card">
        <h1 class="card--title">Maria</h1>
        <li class="topic">Data de Aniversário:</li>
        <li class="topic">Cor Favorita:</li>
        <li class="topic">Comida Favorita:</li>
        <li class="topic">Bebida Favorita:</li>
        <li class="topic">Filme Favorito:</li>
        <li class="topic">Desenho Favorito:</li>
        <li class="topic">Banda/Cantor(a):</li>
      </div>
      <div class="card">
        <h1 class="card--title">Isabelly</h1>
        <li class="topic">Data de Aniversário:</li>
        <li class="topic">Cor Favorita:</li>
        <li class="topic">Comida Favorita:</li>
        <li class="topic">Bebida Favorita:</li>
        <li class="topic">Filme Favorito:</li>
        <li class="topic">Desenho Favorito:</li>
        <li class="topic">Banda/Cantor(a):</li>
      </div>
      <div class="card">
        <h1 class="card--title">Lucas</h1>
        <li class="topic">Data de Aniversário:</li>
        <li class="topic">Cor Favorita:</li>
        <li class="topic">Comida Favorita:</li>
        <li class="topic">Bebida Favorita:</li>
        <li class="topic">Filme Favorito:</li>
        <li class="topic">Desenho Favorito:</li>
        <li class="topic">Banda/Cantor(a):</li>
      </div>
      <div class="card">
        <h1 class="card--title">Diego</h1>
        <li class="topic">Data de Aniversário:</li>
        <li class="topic">Cor Favorita:</li>
        <li class="topic">Comida Favorita:</li>
        <li class="topic">Bebida Favorita:</li>
        <li class="topic">Filme Favorito:</li>
        <li class="topic">Desenho Favorito:</li>
        <li class="topic">Banda/Cantor(a):</li>
      </div>
      <div class="card">
        <h1 class="card--title">Miguel</h1>
        <li class="topic">Data de Aniversário:</li>
        <li class="topic">Cor Favorita:</li>
        <li class="topic">Comida Favorita:</li>
        <li class="topic">Bebida Favorita:</li>
        <li class="topic">Filme Favorito:</li>
        <li class="topic">Desenho Favorito:</li>
        <li class="topic">Banda/Cantor(a):</li>
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
  box-shadow: 1 5px 25px rgba(0, 0, 0, 0.19), 0 6px 6px rgba(0, 0, 0, 0.23);
  border-radius: 15px;
  margin: 25px auto;
  overflow: hidden;
  background-color: rgb(114, 46, 177);
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