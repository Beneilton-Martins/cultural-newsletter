<script setup lang="ts">
const isMenuOpen = ref(false)

function toggleMenu() {
  const navbarMenu = document.querySelector('.navbar-menu')
  if (isMenuOpen.value) {
    isMenuOpen.value = false
    navbarMenu?.classList.remove('open')
  } else {
    isMenuOpen.value = true
    navbarMenu?.classList.add('open')
  }
}
</script>

<template>
  <div>
    <nav class="navbar">
      <div class="menu-toggle" @click="toggleMenu"> Project K </div>
      <div class="navbar-menu">
        <a href="#" class="navbar-item"> Início</a>
        <a href="#" class="navbar-item"> Notícias</a>
        <a href="#" class="navbar-item"> Contato</a>
      </div>
    </nav>
  </div>
</template>

<style scoped>
.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: var(--color-blue);
  color: #FFFFFF;
  padding: 16px 32px;
  user-select: none;
}

.menu-toggle {
  font-weight: bold;
  cursor: pointer;

}

.navbar-menu {
  display: flex;
  gap: 16px;
  background-color: var(--color-blue);
  user-select: none;
}

.navbar-item {
  font-weight: bold;
  color: #FFFFFF;
  text-decoration: none;
  padding: 8px;
}

@media (max-width: 600px) {
  .navbar-menu {
    flex-direction: column;
    align-items: flex-start;
    position: fixed;
    top: calc(0% + 60px);
    bottom: 0;
    left: -100%;
    width: 50%;
    z-index: 1;
    transition: left 0.3s ease-in-out;
  }

  nav .open {
    left: 0;
  }

  .menu-toggle {
    display: block;
  }

  .navbar-item {
    padding: 16px 32px;
    
  }
}
</style>
