<template>
  <section class="ecommerce-content">
    <div class="ecommerce-header">
      <div class="search-results">27 results found</div>
    </div>
    <div class="searchbar">
      <input type="text" v-model="search" placeholder="Search Product" />
      <span class="material-icons-outlined"> search </span>
    </div>

    <!-- products content -->
    <section class="products-view">
      <div v-for="prod in filterProducts" :key="prod.id" class="card">
        <div class="item-img">
          <a href="#">
            <img :src="prod.img" :alt="prod.name" :style="{ width: '200px' }" />
          </a>
        </div>
        <div class="card-body">
          <div class="item-rating">
            <ul>
              <li><span class="material-icons"> star </span></li>
              <li><span class="material-icons"> star </span></li>
              <li><span class="material-icons"> star </span></li>
              <li>
                <span class="material-icons-outlined"> star_border </span>
              </li>
            </ul>
          </div>
          <h5 class="item-price">${{ prod.price }}</h5>
          <div class="item-details">
            <h4 class="item-title">{{ prod.name }}</h4>
            <p class="item-description">{{ prod.discription }}</p>
          </div>
        </div>
        <div class="item-options">
          <a href="#" class="wishlist">
            <span class="material-icons-outlined"> favorite_border </span>
            <span>Wishist</span>
          </a>
          <a href="#" class="addCart">
            <span class="material-icons-outlined"> shopping_cart </span>
            <span>View In Cart</span>
          </a>
        </div>
      </div>
    </section>
  </section>
</template>

<script>
import "../data/store-data.json";

export default {
  name: "search-bar",

  data() {
    return {
      products: [],
      search: "",
    };
  },

  created() {
    fetch("http://localhost:3000/products")
      .then((res) => res.json())
      .then((data) => (this.products = data))
      .catch((error) => console.log(error.message));
  },

  computed: {
    filterProducts: function () {
      return this.products.filter((prod) => {
        return prod.name.toLowerCase().includes(this.search.toLowerCase());
      });
    },
  },
};
</script>

<style scoped>
.ecommerce-content {
  display: flex;
  justify-content: center;
  align-items: center;
}

.ecommerce-header {
  justify-content: center;
  display: flex;
  justify-content: space-between;
  position: absolute;
  top: 28%;
  right: 45%;
}

.search-results {
  font-size: 14px;
  font-weight: 500;
  color: #5e5873;
}

.searchbar {
  display: flex;
  justify-content: center;
  background-color: #fff;
  position: absolute;
  top: 219px;
  right: 39px;
  border: 3px solid #fff;
  border-radius: 4px;
  box-shadow: 0 2px 8px 0 rgb(34 41 47 / 14%);
  margin-left: 10px;
}

.searchbar input {
  width: 710px;
  height: 42px;
  border: 3px solid #fff;
  outline: none;
}

.searchbar input[placeholder] {
  color: #5e5873;
  font-size: 14px;
  font-weight: 500;
  padding-left: 12px;
}

.searchbar span {
  position: relative;
  top: 12px;
  right: 12px;
  color: #b9b9c3;
  font-size: 21px;
}

.products-view {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  grid-gap: 30px;
  margin: 280px auto;
  width: 220px;
  height: 200px;
  padding: 10px;
}

.card {
  box-shadow: 0 5px 5px rgba(0, 0, 0, 0.2);
  background-color: #fff;
  border-radius: 8px;
  width: 230px;
  transition: 0.4s all ease-in-out;
}

.card:hover {
  transform: scale(1.05);
  box-shadow: 0 2px 8px 0 rgb(34 41 47 / 30%);
}

.item-rating ul {
  list-style-type: none;
  display: flex;
  justify-content: flex-start;
}

.item-rating span {
  font-size: 19px;
  color: #ff9f43;
  margin-left: 5px;
}

.item-details .item-title {
  padding-top: 10px;
  padding-bottom: 10px;
  margin-top: -15px;
  margin-left: 11px;
  font-weight: 600;
  font-size: 14px;
  text-align: left;
  text-transform: capitalize;
  color: #6e6b7b;
  overflow: hidden;
  white-space: nowrap;
  text-overflow: ellipsis;
}

.item-img {
  padding: 30px 0;
}

.item-details .item-title:hover {
  color: #7367f0;
  cursor: pointer;
}

.item-details .item-description {
  text-align: left;
  overflow: hidden;
  white-space: nowrap;
  text-overflow: ellipsis;
  font-size: 12px;
  color: #6e6b7b;
  margin-left: 11px;
}

.item-price {
  text-align: right;
  font-weight: 600;
  color: #6e6b7b;
  font-size: 14px;
  position: relative;
  bottom: 22px;
  margin-right: 12px;
}

.item-options a {
  text-decoration: none;
  color: #6e6b7b;
  font-weight: 500;
  display: block;
  padding: 10px;
}

.wishlist {
  text-align: center;
  font-size: 14px;
  padding: 11px 20px;
  margin-top: 20px;
  color: #2a2e30;
  background-color: #f6f6f6;
}

.wishlist:hover {
  background-color: rgb(235, 232, 232);
}

.wishlist span {
  color: #2a2e30;
  font-size: 15px;
  padding-left: 5px;
}

.addCart {
  text-align: center;
  font-size: 14px;
  padding: 5px 0;
  background-color: #7367f0;
  border-bottom-left-radius: 5px;
  border-bottom-right-radius: 5px;
}

.addCart span {
  color: #fff;
  font-size: 15px;
  padding-left: 5px;
}
</style>
