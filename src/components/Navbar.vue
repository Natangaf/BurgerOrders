<template>
  <div>
    <div id="nav">
      <router-link id="logo-url" to="/">
        <img id="logo" :src="logo" :alt="alt">
        <h1>BurgerOrders</h1>
      </router-link>
      <router-link to="/">Fazer Pedido</router-link>
      <router-link to="/pedidos">Pedidos</router-link>
    </div>
  </div>
</template>
  
<script>

export default {
  name: "Navbar",
  props: ["logo", "alt"]
}
</script>
  
<style scoped>
#nav {
  background-color: #222;
  border-bottom: 4px solid #111;
  padding: 15px 50px;
  display: flex;
  justify-content: flex-end;
  align-items: center;
}

#nav h1 {
  color: #FFF;
  font-size: 30px;
}

#nav #logo-url {
  margin: auto;
  margin-left: 0;

  display: flex;
  flex-direction: row;
  align-items: center;
  gap: 20px;

}

#logo {
  width: 40px;
  height: 40px;
}

#nav a {
  color: #fcba03;
  text-decoration: none;
  margin: 12px;
  transition: .5s;
}

#nav a:hover {
  color: #FFF;
}
</style>