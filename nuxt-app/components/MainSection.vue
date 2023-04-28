<!-- MainSection.vue -->
<template>
    <div class="hero-section">
        <h1>Minha Página Inicial</h1>
        <p>Bem-vindo ao meu site!</p>
        <button class="cta-button">Saiba mais</button>
    </div>
</template>
  
<style scoped>
.hero-section {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    margin-top: 32px;
}

.hero-section h1 {
    font-size: 36px;
    font-weight: bold;
    text-align: center;
    margin-bottom: 16px;
}

.hero-section p {
    font-size: 24px;
    text-align: center;
    margin-bottom: 32px;
}

.cta-button {
    background-color: var(--color-green);
    color: #FFFFFF;
    border: none;
    border-radius: 4px;
    padding: 8px 16px;
    cursor: pointer;
    font-size: 18px;
    font-weight: bold;
}
</style>  