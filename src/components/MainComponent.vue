<template>
  <div class="principal">
    <div class="saldo-total">
      <p style="margin-bottom: -20px;">Saldo total</p>
      <div class="saldo-info">
        <p class="valor-saldo" style="font-size: 2rem;">R$ 5000</p>
        <div class="rendimento">
          <i class="fas fa-bolt" style="color: yellow;"></i>
          <p>Rendendo 124%</p>
        </div>
        <div class="botoes" >
          <button class="enviar">Enviar dinheiro</button>
          <button class="adicionar">+</button>
        </div>
      </div>
      <div class="statistics-panel">
        <i class="fas fa-circle-notch"></i>

        <span class="panel-title">Painel de Estatísticas</span>
        <span class="last-days">Últimos 7 dias</span>
      </div>

    </div>



    <div class="panels-container">
      <div>
        <PainelPj />
      </div>
      <div>
        <PainelRecebimentos />
      </div>
      <div>
        <PainelLucro />
      </div>
    </div>
  </div>
  <div class="transaction-analysis-container">
    <div>
      <TransacoesRecentes />
    </div>
    <div>
      <AnaliseGeral />
    </div>
  </div>
</template>

<script>
import PainelPj from './PainelPj.vue';
import PainelLucro from './PainelLucro.vue';
import PainelRecebimentos from './PainelRecebimentos.vue';
import AnaliseGeral from './AnaliseGeral.vue';
import TransacoesRecentes from './TransacoesRecentes.vue';
import '@fortawesome/fontawesome-free/css/all.css';

export default {
  components: {
    PainelPj,
    PainelLucro,
    PainelRecebimentos,
    AnaliseGeral,
    TransacoesRecentes,
  },
}
</script>

<style scoped>
.principal {
  margin-left: 50px;
}

.panels-container {
  display: flex;
  align-items: flex-start;
  flex-direction: row;
  justify-content: space-around;
}

.transaction-analysis-container {
  display: flex;
  align-items: flex-start;
  justify-content: space-around;
  margin-top: 20px;
}

.saldo-total p,
.painel-estatisticas p {
  color: white;
}

.saldo-total {
  display: flex;
  flex-direction: column;
  justify-content: flex-start;
  align-items: flex-start;
}

.saldo-info {
  display: flex;
  align-items: center;
}

.rendimento {
  display: flex;
  align-items: center;
}

.botoes {
  margin-top: 10px;
  display: flex;
  align-items: center;
  justify-content: flex-start;
  margin-left: 800px;
}




.botoes button {
  background-color: #add8e6;
  color: white;
  border: none;
  border-radius: 4px;
  padding: 8px 16px;
  cursor: pointer;
}

.botoes button.adicionar {
  margin-left: 5px;
}

.statistics-panel {
  display: flex;
  align-items: center;
  margin-top: 30px;
}

.statistics-panel i {
  color: red;
  font-size: 16px;
}

.panel-title {
  margin-left: 5px;
  font-weight: bold;
}

.last-days {
  margin-left: 10px;
  color: gray;
}

</style>
