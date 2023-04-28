<template>
  <div>
    <nav class="navbar">
      <div class="navbar-brand">Project K</div>
      <div class="navbar-menu">
        <a href="#" class="navbar-item">Início</a>
        <a href="#" class="navbar-item">Notícias</a>
        <a href="#" class="navbar-item">Contato</a>
      </div>
    </nav>
  </div>
</template>

<style scoped>
.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: #38ABC8;
  color: #FFFFFF;
  padding: 16px;
}

.navbar-brand {
  font-size: 24px;
  font-weight: bold;
}

.navbar-menu {
  display: flex;
  gap: 16px;
}

.navbar-item {
  font-size: 18px;
  font-weight: bold;
  color: #FFFFFF;
  text-decoration: none;
  padding: 8px;
  border-radius: 4px;
}
</style>

