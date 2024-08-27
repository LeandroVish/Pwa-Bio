<script setup>
</script>

<template>
  <div>
    <h1>Friends</h1>
    <div class="container">
      <div class="card">
        <h1 class="card--title">Livia</h1>
        <li class="topic">Data de Aniversário: 22/08</li>
        <li class="topic">Cor Favorita: Vermelho</li>
        <li class="topic">Comida Favorita: Escondidinho de Carne</li>
        <li class="topic">Bebida Favorita: Pepsi</li>
        <li class="topic">Filme Favorito: Coraline e o Mundo Secreto</li>
        <li class="topic">Desenho Favorito: Hora de Aventura</li>
        <li class="topic">Banda/Cantor(a): Vídeo Club</li>
      </div>
      <div class="card">
        <h1 class="card--title">Brian</h1>
        <li class="topic">Data de Aniversário: 13/10</li>
        <li class="topic">Cor Favorita: Amarelo</li>
        <li class="topic">Comida Favorita: Strogonoff da Mãe</li>
        <li class="topic">Bebida Favorita: Milk Shake de Ovomaltine</li>
        <li class="topic">Filme Favorito: Detetive Pikachu</li>
        <li class="topic">Desenho Favorito: Pokémon</li>
        <li class="topic">Banda/Cantor(a): Meu Funeral</li>
      </div>
      <div class="card">
        <h1 class="card--title">Rafael</h1>
        <li class="topic">Data de Aniversário: 15/08</li>
        <li class="topic">Cor Favorita: Preto</li>
        <li class="topic">Comida Favorita: Pizza</li>
        <li class="topic">Bebida Favorita: Coca</li>
        <li class="topic">Filme Favorito: Gente Grande</li>
        <li class="topic">Desenho Favorito: Scooby Doo</li>
        <li class="topic">Banda/Cantor(a): Tame Impala</li>
      </div>
      <div class="card">
        <h1 class="card--title">Duda</h1>
        <li class="topic">Data de Aniversário: 26/12</li>
        <li class="topic">Cor Favorita: Vermelho Escuro</li>
        <li class="topic">Comida Favorita: Sushi</li>
        <li class="topic">Bebida Favorita: Guaraná</li>
        <li class="topic">Filme Favorito: Harry Potter</li>
        <li class="topic">Desenho Favorito: Como Treinar seu Dragão</li>
        <li class="topic">Banda/Cantor(a): The Weeknd</li>
      </div>
      <div class="card">
        <h1 class="card--title">Leandro</h1>
        <li class="topic">Data de Aniversário: 23/05</li>
        <li class="topic">Cor Favorita: Laranja</li>
        <li class="topic">Comida Favorita: Espaguete</li>
        <li class="topic">Bebida Favorita: Caldo de Cana</li>
        <li class="topic">Filme Favorito: De Volta Pro Futuro</li>
        <li class="topic">Desenho Favorito: Thundercats</li>
        <li class="topic">Banda/Cantor(a): Luan Santana</li>
      </div>
      <div class="card">
        <h1 class="card--title">Maria</h1>
        <li class="topic">Data de Aniversário: 09/02</li>
        <li class="topic">Cor Favorita: Verde</li>
        <li class="topic">Comida Favorita: ???</li>
        <li class="topic">Bebida Favorita: Guaraná</li>
        <li class="topic">Filme Favorito: 10 Coisas Que Eu Odeio Em Você</li>
        <li class="topic">Desenho Favorito: Monster High</li>
        <li class="topic">Banda/Cantor(a): Cbjr / Ajuliacosta</li>
      </div>
      <div class="card">
        <h1 class="card--title">Isabelly</h1>
        <li class="topic">Data de Aniversário: 15/04</li>
        <li class="topic">Cor Favorita: Verde</li>
        <li class="topic">Comida Favorita: Empadão de Frango da Mãe</li>
        <li class="topic">Bebida Favorita: Café</li>
        <li class="topic">Filme Favorito: Rei Leão</li>
        <li class="topic">Desenho Favorito: Looney Tunes</li>
        <li class="topic">Banda/Cantor(a): Rodolfo Abrantes</li>
      </div>
      <div class="card">
        <h1 class="card--title">Lucas</h1>
        <li class="topic">Data de Aniversário: 02/05</li>
        <li class="topic">Cor Favorita: Preto</li>
        <li class="topic">Comida Favorita: Aipim Frito / Macarrão</li>
        <li class="topic">Bebida Favorita: Suco de Melancia</li>
        <li class="topic">Filme Favorito: Whiplash</li>
        <li class="topic">Desenho Favorito: Steven Universo</li>
        <li class="topic">Banda/Cantor(a): Cbjr</li>
      </div>
      <div class="card">
        <h1 class="card--title">Diego</h1>
        <li class="topic">Data de Aniversário: 11/01</li>
        <li class="topic">Cor Favorita: Preto</li>
        <li class="topic">Comida Favorita: Churrasco</li>
        <li class="topic">Bebida Favorita: Guaraná</li>
        <li class="topic">Filme Favorito: Cavalos de Guerra</li>
        <li class="topic">Desenho Favorito: Gumball</li>
        <li class="topic">Banda/Cantor(a): Grupo Cordiona</li>
      </div>
      <div class="card">
        <h1 class="card--title">Miguel</h1>
        <li class="topic">Data de Aniversário: 27/08</li>
        <li class="topic">Cor Favorita: Preto/Roxo</li>
        <li class="topic">Comida Favorita: Macarrão</li>
        <li class="topic">Bebida Favorita: Guaraná</li>
        <li class="topic">Filme Favorito: Por Lugares Incriveis</li>
        <li class="topic">Desenho Favorito: Futurama</li>
        <li class="topic">Banda/Cantor(a): Baco Exu od Blues</li>
      </div>
    </div>
  </div>
</template>
<style>
@property --rotate {
    syntax: "<angle>";
    initial-value: 132deg;
    inherits: false;
  }

  :root {
    --card-height: 65vh;
    --card-width: calc(var(--card-height) / 1.5);
  }

  body {
    min-height: 100vh;
    background: #212534;
    display: flex;
    align-items: center;
    flex-direction: column;
    padding-top: 2rem;
    padding-bottom: 2rem;
    box-sizing: border-box;
  }

  .card {
    background: #191c29;
    width: var(--card-width);
    height: var(--card-height);
    padding: 3px;
    position: relative;
    flex-direction: column;
    border-radius: 8px;
    justify-content: space-between;
    align-items: center;
    text-align: center;
    display: flex;
    font-size: 1.5em;
    color: rgb(88 199 250 / 0%);
    cursor: pointer;
    font-family: cursive;
    margin: 10px auto;
  }

  .card:hover {
    color: rgb(88 199 250 / 100%);
    transition: color 1s;
  }

  .card:hover:before,
  .card:hover:after {
    animation: none;
    opacity: 0;
  }

  .card::before {
    content: "";
    width: 104%;
    height: 102%;
    border-radius: 12px;
    background-image: linear-gradient(var(--rotate),
        #5ddcff,
        #3c67e3 43%,
        #4e00c2);
    position: absolute;
    z-index: -1;
    top: -1%;
    left: -2%;
    animation: spin 2.5s linear infinite;
  }

  .card::after {
    position: absolute;
    content: "";
    top: calc(var(--card-height) / 6);
    left: 0;
    right: 0;
    z-index: -1;
    height: 100%;
    width: 100%;
    margin: 0 auto;
    transform: scale(0.8);
    filter: blur(calc(var(--card-height) / 6));
    background-image: linear-gradient(var(--rotate),
        #5ddcff,
        #3c67e3 43%,
        #4e00c2);
    opacity: 1;
    transition: opacity 0.5s;
    animation: spin 2.5s linear infinite;
  }

  @keyframes spin {
    0% {
      --rotate: 0deg;
    }

    100% {
      --rotate: 360deg;
    }
  }

  a {
    color: #212534;
    text-decoration: none;
    font-family: sans-serif;
    font-weight: bold;
    margin-top: 1.5rem;
  }
  .card--title {
  color:rgb(88 199 250 / 100%) ;
  font-weight: 700;
  text-transform: capitalize;
  font-size: 1.1rem;
  margin-top: 0.5rem;
}
.card--avatar {
  width: 100%;
  height: 17rem;
  object-fit: cover;
  margin-bottom: 0.5rem;
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
</style>