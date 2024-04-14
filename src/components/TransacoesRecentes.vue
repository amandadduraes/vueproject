<template>
    <div class="card">
      <div class="header">
        <h2 class="title">Transações recentes</h2>
        <p class="subtitle">Últimos 7 dias</p>
        <a href="#" class="link">Ver tudo</a>
      </div>
      <hr>
      <div class="transaction">
        <div class="icon yellow-bg">
          <i class="fas fa-store fa-sm"></i>
        </div>
        <div class="transaction-details">
          <p class="detail">Mercadinho da cidade</p>
          <p class="price">R$ 10,98</p>
        </div>
      </div>
      <hr>
      <div class="transaction">
        <div class="icon red-bg">
          <i class="fas fa-store fa-sm"></i>
        </div>
        <div class="transaction-details">
          <p class="detail">Tenda Nostra</p>
          <p class="price">R$ 26,38</p>
        </div>
      </div>
      <hr>
      <div class="transaction">
        <div class="icon green-bg">
          <i class="fas fa-store fa-sm"></i>
        </div>
        <div class="transaction-details">
          <p class="detail">Farmácia um</p>
          <p class="price">R$ 43,17</p>
        </div>
      </div>
      <hr>
      <div class="transaction">
        <div class="icon purple-bg">
          <i class="fas fa-store fa-sm"></i>
        </div>
        <div class="transaction-details">
          <p class="detail">Academia Body</p>
          <p class="price">R$ 62,12</p>
        </div>
      </div>
      <hr>
      <div class="transaction">
        <div class="icon pink-bg">
          <i class="fas fa-store fa-sm"></i>
        </div>
        <div class="transaction-details">
          <p class="detail">ShopOnline</p>
          <p class="price">R$ 135,24</p>
        </div>
      </div>
    </div>
  </template>
  
  <style scoped>
  .card {
    border: none;
    border-radius: 1px;
    padding: 10px;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
    width: 350px;
    height: auto;
  }
  
  .header {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  
  .title {
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
  }
  
  .transaction {
    display: flex;
    align-items: center;
    height: 30px;
    overflow: hidden;
  }
  
  .transaction-details {
    font-size: 0.6rem;
    display: flex;
    justify-content: space-between; 
    align-items: center;
    flex: 1;
  }
  
  .detail {
    margin-right: 10px;
  }
  
  .icon {
    width: 20px;
    height: 20px;
    margin-right: 10px;
  }
  
  .yellow-bg {
    background-color: yellow;
  }
  
  .red-bg {
    background-color: red;
  }
  
  .green-bg {
    background-color: green;
  }
  
  .purple-bg {
    background-color: purple;
  }
  
  .pink-bg {
    background-color: pink;
  }
  </style>
  