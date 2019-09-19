<template>
  <section id="navbar">
    <div class="shop">
      <div class="home">
        <router-link to="/">Home</router-link>
      </div>
      <div id="shop">
        <router-link to="/shop">Shop</router-link>
      </div>
    </div>
    <div class="brand">Bass Line</div>
    <div class="user">
      <div class="account">Account</div>
      <div class="cart">
        <router-link to="/cart">Cart</router-link>
      </div>
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style scoped>
@font-face {
  font-family: "UndergroundNF";
  src: url("../assets/UndergroundNF.ttf") format("truetype");
}

#navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: #eee;
  height: 10vh;
}

.shop {
  display: flex;
  align-items: center;
}

.shop div {
  padding: 0 20px;
}

.brand {
  font-family: "UndergroundNF";
  font-size: 8vh;
  flex-grow: 1;
  display: flex;
  justify-content: center;
  align-items: center;
}

.user {
  display: flex;
  align-items: center;
}

.user div {
  padding: 0 20px;
}
</style>
