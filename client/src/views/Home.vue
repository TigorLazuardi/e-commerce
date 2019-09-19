<template>
  <div class="container">
    <div class="home">
      <p class="brand">Bass Line</p>
      <h1>
        fulfill your dream
        <br />and slapp the bass
      </h1>
      <router-link to="/shop" id="go-shop">Shop Now</router-link>
    </div>
  </div>

  <!-- v-bind:style="{ 'background-image': 'url(' + image + ')' } -->
</template>

<script>
// @ is an alias to /src

export default {
  name: "home",
  data: {
    image: "../assets/bassist-min.jpg"
  }
};
</script>

<style scoped>
@font-face {
  font-family: "UndergroundNF";
  src: url("../assets/UndergroundNF.ttf") format("truetype");
}

.container {
  display: flex;
  min-height: 100vh;
}

.home {
  flex-grow: 1;
  background-image: url("../assets/bass-guitar-min.jpg");
  background-size: cover;
  background-repeat: no-repeat;
  color: white;
  display: flex;
  flex-direction: column;
  align-items: flex-end;
  justify-content: center;
}

.home > * {
  margin: 5vh 10vw;
}

.brand {
  font-family: "UndergroundNF";
  font-size: 8vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-shadow: 0 0 10px #e38e1e;
}

.home > h1 {
  text-align: end;
  text-shadow: 0 0 10px #e38e1e;
  text-transform: uppercase;
}

#go-shop {
  color: white;
  border: 5px solid white;
  padding: 1vw;
  border-radius: 25px;
  font-weight: bold;
  text-shadow: 0 0 10px #e38e1e;
  text-transform: uppercase;
}

#go-shop:hover {
  color: #1c5f92;
  border: 5px solid #1c5f92;
  background-color: white;
  text-shadow: 0 0 0 #1c5f92;
  animation-name: pulse;
  animation: ease-in-out;
  animation-duration: 1s;
}

@keyframes pulse {
  0% {
    transform: scale(1);
  }
  50% {
    transform: scale(1.1);
  }
  100% {
    transform: scale(1);
  }
}
</style>