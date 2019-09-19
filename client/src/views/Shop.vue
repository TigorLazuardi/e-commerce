<template>
  <div id="shop">
    <nav-bar />
    <div class="background">
      <div class="container">
        <div class="cards">
          <div class="card-header">
            <div class="image-container">
              <img
                src="https://images.reverb.com/image/upload/s--jvkgTGy3--/t_card-square/v1529423035/cy76blbp3i6ojoqryzlz.png"
                alt="bass"
              />
            </div>
            <h3 class="product-name">Gibson</h3>
            <div class="product-meta">
              <div class="stock">Stock: 10</div>
              <div class="price">Price: Rp10.000.000</div>
              <div class="buy">Buy Button</div>
            </div>
          </div>
          <div class="card-footer">
            <div class="date">
              <p>createdAt</p>
              <p>updatedAt</p>
            </div>
          </div>
        </div>
        <div class="cards"></div>
        <div class="cards"></div>
        <div class="cards"></div>
        <div class="cards"></div>
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
#shop {
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
  justify-content: space-evenly;
  padding: 5vh 3vw;
}

.cards {
  border: 2px solid #c3c0b0;
  width: 300px;
  height: 400px;
  margin: 2vh 2vw;
  border-radius: 10px;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: space-between;
  box-shadow: 0px 0px 16px -3px rgba(0, 0, 0, 0.75);
}

.card-header {
  display: flex;
  flex-direction: column;
  /* align-items: center; */
  width: 100%;
  height: 100%;
  color: #606060;
}

.card-header > * {
  margin: 0 1vh;
}

.image-container {
  flex-grow: 1;
  border-radius: 9px 9px 0 0;
}

.image-container img {
  object-fit: contain;
  max-width: 100%;
  max-height: 100%;
  border-radius: 8px 8px 0 0;
}

.card-footer {
  width: 100%;
}

.card-footer .date {
  display: flex;
  justify-content: space-evenly;
  width: 100%;
}
</style>