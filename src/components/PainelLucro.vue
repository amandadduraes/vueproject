<template>
  <div class="panel-lucro">
    <div class="card">
      <div class="header">
        <h2>Lucro</h2>
      </div>
      <div>
        <div class="content">
        <p class="valor">{{ formattedValue }}</p>
        <button @click="verDetalhes">Ver mais detalhes</button>
      </div>
      <div class="menu-button">
        <button @click="toggleMenu">&#9776;</button>
      </div>
      </div>
      
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      valor: 5000, 
      menuAberto: false
    };
  },
  computed: {
    formattedValue() {
      return `R$ ${this.valor.toFixed(2)}`; 
    }
  },
  methods: {
    verDetalhes() {
      console.log("Ver mais detalhes");
    },
    toggleMenu() {
      this.menuAberto = !this.menuAberto;
    }
  }
};
</script>

<style>
.panel-lucro {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100%;
}

.header {
  text-align: center;
}

.content {
  margin-top: 20px;
}

.menu-button {
  position: absolute;
  top: 10px;
  right: 10px;
}

.menu-button button {
  background: none;
  border: none;
  font-size: 24px;
  cursor: pointer;
}

.valor {
  font-size: 24px; 
  font-weight: bold; 
}
</style>
