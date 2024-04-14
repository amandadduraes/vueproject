<template>
  <div class="menu">
    <div class="brand">BigBang</div>
    <ul>
      <li><router-link to="/">Dashboard</router-link></li>
      <li><router-link to="/pagamentos">Pagamentos</router-link></li>
      <li><router-link to="/invoices">Invoices</router-link></li>
      <li><router-link to="/insights">Insights</router-link></li>
    </ul>
    <div class="notification">
      <i class="fas fa-bell"></i> 
    </div>
  </div>
</template>

<script>
export default {
  name: 'MainMenu',
}
</script>

<style>
.menu {
  display: flex;
  align-items: center;
  justify-content: space-between; 
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  background-color: #333;
  color: white;
  padding: 10px;
}

.brand {
  color: red;
  font-weight: bold;
}

.menu ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  margin: auto; 
}

.menu ul li {
  display: inline-block;
  margin-right: 10px;
}

.menu ul li a {
  color: white;
  text-decoration: none;
}

.notification {
  margin-left: auto; 
  margin-right: 20px;
}
</style>
