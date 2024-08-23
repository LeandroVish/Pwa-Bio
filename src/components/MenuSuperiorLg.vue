<script setup>
  import { ref } from 'vue';

  import CartPlus from 'vue-material-design-icons/CartPlus.vue';
  import Account from 'vue-material-design-icons/Account.vue';
  import Menu from 'vue-material-design-icons/Menu.vue';

  const menuAberto = ref(false);
</script>

<template>
  <header>
    <div class="header--logo">
      <img src="@/assets/logoFakeStore.png" alt="Logo" />
      <h1>Bio</h1>
    </div>
    <nav>

      <!--<ul :class="menuAberto ? 'menu' : 'mobile'">
        <li>Home</li>
        <li>Plus</li>
      </ul> -->

      <!-- TOPBAR -->

      <ul class="c-mobile__topbar">
        <input type="checkbox" id="u-topbar__button" class="u-topbar__button" />
        <label for="u-topbar__button" class="c-button c-topbar__button--menu fa fa-bars"></label>
        <label for="u-topbar__button" class="c-button c-topbar__button--close fa fa-times"></label>
        <ul>
          <li><a href="#" class="u-link__effect">Events list</a></li>
          <li><a href="#" class="u-link__effect">Favorites</a></li>
          <li><a href="#" class="u-link__effect">Credits</a></li>
        </ul>
      </ul>

    </nav>
    <div class="header--icons">
      <Account />
      <CartPlus />
      <Menu class="menu-hamburger" @click="menuAberto = !menuAberto" />
    </div>
  </header>
</template>

<style scoped>
  header {
    background: #fff;
    box-shadow: 0 10px 20px rgba(0, 0, 0, 0.19), 0 6px 6px rgba(0, 0, 0, 0.23);
    padding: 0.2rem 1rem;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  .header--logo {
    display: flex;
    align-items: center;
  }
  .header--logo img {
    width: 3rem;
    height: 3rem;
    margin-right: 0.5rem;
  }
  nav ul {
    display: flex;
    gap: 1rem;
  }
  nav li {
    list-style: none;
  }

  .header--icons {
    display: flex;
    gap: 1rem;
  }
  .menu-hamburger {
    display: none;
  }

  @media (max-width: 768px) {
    nav ul {
      display: none;
    }
    .menu-hamburger {
      display: block;
    }

    nav .menu {
      display: flex;
      flex-direction: column;
      position: absolute;
      background-color: rgba(255, 255, 255, 0.9);
      box-shadow: 0 10px 20px rgba(0, 0, 0, 0.19), 0 6px 6px rgba(0, 0, 0, 0.23);
      border-radius: 10px;
      right: 0;
      text-align: right;
      padding: 10px 16px;
    }
    nav .menu li {
      display: block;
      margin-top: 12px;
    }
  }
  .c-mobile__topbar {
  position: relative;
  overflow: hidden;
  width: 100%;
  height: 10%;
  transition: all 0.3s ease;
  border-radius: 30px 30px 0 100%;
  background: linear-gradient(to right, #ADD8E6, #800080);
}

.c-mobile__topbar a {
  text-decoration: none;
  color: #ffffff;
  letter-spacing: 3px;
  font-size: 1.4em;
  z-index: 1;
  transition: all 0.3s ease;
}

.c-mobile__topbar a:hover {
  color: #FFFF00;
}

.c-mobile__topbar ul {
  text-align: right;
  padding-top: 40px;
}

.c-mobile__topbar li {
  margin: 30px 30px 40px 0;
}

.u-topbar__button:checked~.c-mobile__topbar {
  height: 50%;
  transition: all 0.6s ease;
}
</style>