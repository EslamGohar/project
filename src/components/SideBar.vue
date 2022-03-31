<template>
  <aside class="sidebar">
    <h5 class="filter-heading">Filters</h5>
    <div class="sidebar-body">
      <h5 class="filter-title">Multi Range</h5>
      <div class="multi-range">
        <div class="multi-range-group">
          <input
            type="radio"
            class="custom-control-input"
            value="all"
            checked
          />
          <label>All</label>
        </div>
        <div class="multi-range-group">
          <input type="radio" class="custom-control-input" value="<=10" />
          <label>&lt;= $10</label>
        </div>
        <div class="multi-range-group">
          <input type="radio" class="custom-control-input" value="10-100" />
          <label>$10 - $100</label>
        </div>
        <div class="multi-range-group">
          <input type="radio" class="custom-control-input" value="100-500" />
          <label>$100 - $500</label>
        </div>
        <div class="multi-range-group">
          <input type="radio" class="custom-control-input" value=">=500" />
          <label>&gt;= $500</label>
        </div>
      </div>

      <div class="price-range">
        <h5 class="price-title">Price Range</h5>
        <div class="slidecontainer">
          <input type="range" min="0" max="100" value="50" class="slider" />
        </div>
      </div>

      <h5 class="categories-title">Categories</h5>
      <div class="product-categries">
        <div class="product-categries-group">
          <input
            type="radio"
            class="custom-control-input"
            value="appliances"
            checked
          />
          <label>Appliances</label>
        </div>
        <div class="product-categries-group">
          <input type="radio" class="custom-control-input" value="audio" />
          <label>Audio</label>
        </div>
        <div class="product-categries-group">
          <input
            type="radio"
            class="custom-control-input"
            value="cameras & camcorders"
          />
          <label>Cameras & Camcorders</label>
        </div>
        <div class="product-categries-group">
          <input
            type="radio"
            class="custom-control-input"
            value="car electronics & gps"
          />
          <label>Car Electronics & GPS</label>
        </div>
        <div class="product-categries-group">
          <input
            type="radio"
            class="custom-control-input"
            value="cell phones"
          />
          <label>Cell Phones</label>
        </div>
        <div class="product-categries-group">
          <input
            type="radio"
            class="custom-control-input"
            value="computers & tablets"
          />
          <label>Computers & Tablets</label>
        </div>
        <div class="product-categries-group">
          <input
            type="radio"
            class="custom-control-input"
            value="health, fitness & beauty"
          />
          <label>Health, Fitness & Beauty</label>
        </div>
        <div class="product-categries-group">
          <input
            type="radio"
            class="custom-control-input"
            value="office & school supplies"
          />
          <label>Office & School Supplies</label>
        </div>
        <div class="product-categries-group">
          <input
            type="radio"
            class="custom-control-input"
            value="tv & home theater"
          />
          <label>TV & Home Theater</label>
        </div>
        <div class="product-categries-group">
          <input
            type="radio"
            class="custom-control-input"
            value="Video Games"
          />
          <label>Video Games</label>
        </div>
      </div>

      <h5 class="brands-title">Brands</h5>
      <div class="brands">
        <div class="brands-group">
          <input type="radio" class="custom-control-input" value="Insignia™" />
          <label>Insignia™</label>
        </div>
        <div class="brands-group">
          <input type="radio" class="custom-control-input" value="Samsung" />
          <label>Samsung</label>
        </div>
        <div class="brands-group">
          <input type="radio" class="custom-control-input" value="Metra" />
          <label>Metra</label>
        </div>
        <div class="brands-group">
          <input type="radio" class="custom-control-input" value="HP" />
          <label>HP</label>
        </div>
        <div class="brands-group">
          <input type="radio" class="custom-control-input" value="Apple" />
          <label>Apple</label>
        </div>
        <div class="brands-group">
          <input type="radio" class="custom-control-input" value="Sony" />
          <label>Sony</label>
        </div>
        <div class="brands-group">
          <input type="radio" class="custom-control-input" value="Incipio" />
          <label>Incipio</label>
        </div>
        <div class="brands-group">
          <input type="radio" class="custom-control-input" value="KitchenAid" />
          <label>KitchenAid</label>
        </div>
        <div class="brands-group">
          <input type="radio" class="custom-control-input" value="Whirlpool" />
          <label>Whirlpool</label>
        </div>
      </div>

      <h5 class="rating-title">Ratings</h5>
      <div class="rating-list">
        <ul class="rating-list-items">
          <li>
            <a href="#">
              <span class="material-icons"> star </span>
              <span class="material-icons"> star </span>
              <span class="material-icons"> star </span>
              <span class="material-icons"> star </span>
              <span class="material-icons-outlined"> star_border </span>
              <span class="and-up">& Up</span>
            </a>
            <span class="rating-mount">160</span>
          </li>
          <li>
            <a href="#">
              <span class="material-icons"> star </span>
              <span class="material-icons"> star </span>
              <span class="material-icons"> star </span>
              <span class="material-icons-outlined"> star_border </span>
              <span class="material-icons-outlined"> star_border </span>
              <span class="and-up">& Up</span>
            </a>
            <span class="rating-mount">176</span>
          </li>
          <li>
            <a href="#">
              <span class="material-icons"> star </span>
              <span class="material-icons"> star </span>
              <span class="material-icons-outlined"> star_border </span>
              <span class="material-icons-outlined"> star_border </span>
              <span class="material-icons-outlined"> star_border </span>
              <span class="and-up">& Up</span>
            </a>
            <span class="rating-mount">291</span>
          </li>
          <li>
            <a href="#">
              <span class="material-icons"> star </span>
              <span class="material-icons-outlined"> star_border </span>
              <span class="material-icons-outlined"> star_border </span>
              <span class="material-icons-outlined"> star_border </span>
              <span class="material-icons-outlined"> star_border </span>
              <span class="and-up">& Up</span>
            </a>
            <span class="rating-mount">190</span>
          </li>
        </ul>
      </div>
    </div>
  </aside>
</template>

<script>
export default {
  name: "sidebar-component",
};
</script>

<style scoped>
.sidebar {
  display: flex;
  justify-content: flex-start;
  align-items: center;
  max-height: 60%;
}

.sidebar .filter-heading {
  position: absolute;
  top: 183px;
  left: 292px;
  line-height: 1.2;
  color: #5e5873;
  font-weight: 500;
  font-size: 14px;
  letter-spacing: 0.6px;
}

.sidebar-body {
  width: 19%;
  position: absolute;
  top: 33%;
  left: 21%;
  margin-left: 5px;
  padding: 21px;

  color: #625f6e;
  background-color: #fff;
  box-shadow: 0 4px 24px 0 rgb(34 41 47 / 10%);
  border-radius: 5px;
}

.sidebar-body .filter-title {
  display: flex;
  font-weight: 500;
  font-size: 15px;
}

.multi-range,
.product-categries,
.brands {
  display: block;
  margin-top: 17px;
}

.multi-range-group,
.product-categries-group,
.brands-group {
  display: flex;
  justify-content: flex-start;
}

.multi-range-group label,
.product-categries-group label,
.brands-group label {
  font-size: 14px;
  margin-left: 22px;
  font-weight: 400;
  padding-bottom: 12px;
}

.custom-control-input {
  position: absolute;
  width: 1rem;
  height: 1.225rem;
}

.price-range {
  margin-top: 20px;
  display: flex;
  align-items: center;
}

.price-title {
  font-weight: 500;
  font-size: 15px;
  margin-bottom: 1.3rem;
  margin-top: 0.3rem;
}

.slidecontainer {
  width: 95%;
  position: absolute;
  right: 7px;
}

.slider {
  -webkit-appearance: none;
  appearance: none;
  width: 90%;
  height: 5px;
  margin-top: 55px;
  background: #d3d3d3;
  outline: none;
  border-radius: 8px;
  opacity: 0.7;
  -webkit-transition: 0.2s;
  transition: opacity 0.2s;
}
.slider:hover {
  opacity: 1;
}

.categories-title {
  display: flex;
  font-weight: 500;
  font-size: 15px;
  margin-top: 40px;
}

.brands-title,
.rating-title {
  display: flex;
  font-weight: 500;
  font-size: 15px;
  margin-top: 22px;
}

.rating-list {
  display: flex;
  justify-content: flex-start;
}

.rating-list-items {
  list-style: none;
  margin-top: 12px;
}

.rating-list-items a {
  text-decoration: none;
  color: #ff9f43;
  font-size: 14px;
}

span.and-up {
  color: #7367f0;
  font-size: 14px;
  text-transform: lowercase;
  position: absolute;
  padding: 4px;
}

span.rating-mount {
  position: absolute;
  right: 14px;
  font-size: 14px;
  padding: 5px 3px;
}
</style>
