<template>
  <div id="cart">
    <nav-bar />
    <div class="background">
      <div class="container">
        <div class="table">
          <div class="table-head">
            <p>Product</p>
            <p>Price</p>
            <p>Quantity</p>
          </div>
          <div class="table-row1">
            <p>Gibson</p>
            <p>Rp10.000.000</p>
            <p>1</p>
          </div>
          <!-- <div class="table-row2"></div>
          <div class="table-row3"></div>-->
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import navBar from "../components/NavBar";
export default {
  components: {
    navBar
  }
};
</script>

<style scoped>
#cart {
  display: flex;
  flex-direction: column;
}

.background {
  flex-grow: 1;
  min-height: 90vh;
  background-color: #606060;
  color: #c3c0b0;
}

.container {
  width: 95%;
  margin: 5vh auto;
  min-height: 80vh;
  background-color: white;
  border-radius: 1em;
  display: flex;
  flex-wrap: wrap;
  align-content: center;
  justify-content: center;
  padding: 5vh 3vw;
  color: #606060;
}

.table,
.table > div {
  display: flex;
}

.table {
  flex-direction: column;
  width: inherit;
  /* border: 1px dashed black; */
}

.table > div {
  justify-content: space-between;
  align-items: center;
  width: 100%;
  border: 1px dashed black;
  flex-wrap: wrap;
  flex-basis: 25%;
}

.table > div > p {
  width: 33%;
  border: 1px dashed black;
}

.table > div > p:first-child {
  /* flex-grow: 1; */
}
</style>