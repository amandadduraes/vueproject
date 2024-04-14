<template>
    <div class="analise-geral">
      <div class="titulo">
        <h2 class="title">Análise Geral</h2>
        <span class="subtitle">Nos últimos 7 dias</span>
        <button class="link">Ver tudo</button>
      </div>
      <hr class="linha-divisoria">
      <div class="ganhos-saidas">
        <div class="item">
          <span class="rotulo">Ganhos</span>
          <div class="valor-ganhos">R$ <span class="negrito">5000</span></div>
        </div>
        <div class="item">
          <span class="rotulo">Saídas</span>
          <div class="valor-saidas">R$ <span class="negrito">3000</span></div>
        </div>
      </div>
      <hr class="linha-divisoria">
      <div class="categoria-com-progresso">
        <div class="categoria">
          <i class="fas fa-shopping-cart"></i>
          <span class="titulo-categoria">Compras</span>
          <span class="porcentagem">50%</span>
        </div>
        <div class="barra-progresso">
          <div class="progresso" style="width: 50%;"></div>
        </div>
      </div>
      <div class="categoria-com-progresso">
        <div class="categoria">
          <i class="fas fa-file-invoice-dollar"></i>
          <span class="titulo-categoria">Boletos</span>
          <span class="porcentagem">30%</span>
        </div>
        <div class="barra-progresso">
          <div class="progresso" style="width: 30%;"></div>
        </div>
      </div>
      <div class="categoria-com-progresso">
        <div class="categoria">
          <i class="fas fa-chart-line"></i>
          <span class="titulo-categoria">Investimentos</span>
          <span class="porcentagem">20%</span>
        </div>
        <div class="barra-progresso">
          <div class="progresso" style="width: 20%;"></div>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'AnaliseGeral',
  }
  </script>
  
  <style scoped>
  .analise-geral {
    background-color: #ffffff;
    padding: 20px;
    border-radius: 1px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    width: 350px;
    height: auto;
  }
  .titulo {
    display: flex;
    justify-content: space-between;
    align-items: center;
    font-size: 1rem;
  }
  .subtitle {
    font-size: 0.6rem;
    color: #888;
  }
  .link {
    font-size: 0.6rem;
    color: blue;
    text-decoration: none;
    background: none;
    border: none;
  }
  .linha-divisoria {
    margin: 20px 0;
  }
  .title {
    font-size: 1rem;
  }
  .ganhos-saidas {
    display: flex;
    justify-content: space-between;
  }
  .item {
    text-align: center;
  }
  .valor-ganhos,
  .valor-saidas {
    text-align: center;
    font-weight: bold;
    font-size: 1.2rem;
  }
  .negrito {
    font-weight: bold;
  }
  .categoria-com-progresso {
    margin-top: 20px;
  }
  .categoria {
    display: flex;
    align-items: center;
  }
  .titulo-categoria {
    margin-left: 10px;
  }
  .porcentagem {
    margin-right: 10px;
  }
  .barra-progresso {
    height: 8px;
    background-color: #f2f2f2;
    border-radius: 4px;
    overflow: hidden;
    margin-top: 10px;
  }
  .progresso {
    width: 100%;
    height: 100%;
    background-color: #007bff;
  }
  </style>
  