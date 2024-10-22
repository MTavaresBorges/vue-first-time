<!-- Estrutura extraída do site: https://vuejs.org/guide/scaling-up/routing.html -->

<!-- SCRIPT -->
<script setup>
  // Importações do Vue
    import { ref, computed } from 'vue'

    // Páginas
    import Page1 from './Page1.vue'
    import Page2 from './Page2.vue'
    import ErrorPage from './ErrorPage.vue'

    // Criar uma estrutura de rotas, contendo o caminho e o camponente
    const routes = {
        '/': Page1,
        '/page2': Page2,
        '/404': ErrorPage
    }

    // Obter o conteúdo a partir da cerquila, exemplo: http://localhost:5173/#/sobre o retorno será: #/sobre
    const routeRef = ref(window.location.hash)

    // Executa a ação quando realizar a navegação entre páginas. Obter o conteúdo a partir da cerquilha
    window.addEventListener('hashchange', () => {
        routeRef.value = window.location.hash
    });

    // Função responsável por exibir a página específica
    const currentView = computed(() => {
        return routes[routeRef.value.slice(1) || '/'] || ErrorPage
    })
</script>

<!-- TEMPLATE -->
<template>
    <!-- Links -->
    <a href="#/">Page 1</a>
    |
    <a href="#/page2">Page 2</a>

    <!-- Exibição das páginas -->
    <component :is="currentView" />
</template>