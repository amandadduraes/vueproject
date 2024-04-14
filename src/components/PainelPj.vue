<template>
  <div class="panel-pj">
    <div class="card">
      <div class="header">
        <h2>Conta PJ</h2>
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
      valor: 1000,
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
.panel-pj {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100%;
}

.card {
  border: 1px solid #ccc;
  border-radius: 1px;
  width: 300px;
  padding: 20px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  position: relative; 
  background: white;
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
