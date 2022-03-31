<template>
  <nav class="navbar">
    <div class="navbar-logo">
      <a href="#">
        <img src="../assets/logo.svg" alt="brand-logo" />
        <h2 class="navbar-title">Vuexy</h2>
      </a>
    </div>
    <a href="#" class="navbar-toggle-icon">
      <span class="material-icons-outlined"> adjust </span>
    </a>

    <ul class="navbar-menu">
      <li>
        <a href="#">
          <span class="material-icons-outlined"> home </span>
          <span>Dashboards</span>
          <div class="badge">2</div>
          <span class="material-icons-outlined"> navigate_next </span>
        </a>

        <ul class="dropdown-list">
          <li class="list-item">
            <a href="#">
              <span class="list-title">eCommerce</span>
            </a>
          </li>

          <li class="list-item">
            <a href="#">
              <span class="list-title">Analytics</span>
            </a>
          </li>
        </ul>
      </li>
    </ul>

    <div class="apps-pages">
      <span class="apps-title">apps & pages</span>
      <ul class="apps-items">
        <li>
          <a href="#" class="item-icons">
            <span class="material-icons-outlined"> email </span>
            <span>Email</span>
          </a>
        </li>
        <li>
          <a href="#" class="item-icons">
            <span class="material-icons-outlined">chat_bubble_outline</span>
            <span>Chat</span>
          </a>
        </li>
        <li>
          <a href="#" class="item-icons">
            <span class="material-icons-outlined"> checklist </span>
            <span>Todo</span>
          </a>
        </li>
        <li>
          <a href="#" class="item-icons">
            <span class="material-icons-outlined"> calendar_today </span>
            <span>Calender</span>
          </a>
        </li>
        <li>
          <a href="#" class="item-icons">
            <span class="material-icons-outlined"> description </span>
            <span>Invoice</span>
          </a>
        </li>
        <li>
          <a href="#" class="item-icons">
            <span class="material-icons-outlined"> shopping_cart </span>
            <span>eCommerce</span>
          </a>
        </li>
        <li>
          <a href="#" class="item-icons">
            <span class="material-icons-outlined"> person_outline </span>
            <span>User</span>
          </a>
        </li>
      </ul>
    </div>
  </nav>
</template>

<script>
export default {
  name: "navbar-component",
};
</script>

<style scoped>
.navbar {
  width: 265px;
  height: 100%;
  position: fixed;
  background-color: #fff;
  box-shadow: 0 0 15px 0 rgb(34 41 47 / 5%);
  z-index: 999;
}

.navbar-logo {
  display: flex;
  align-items: center;
  padding-top: 25px;
}

.navbar-logo a {
  display: flex;
  text-decoration: none;
  padding-left: 20px;
}

.navbar-logo img {
  max-width: 38px;
}

.navbar-title {
  padding-left: 14px;
  font-weight: 600;
  font-size: 1.3rem;
  letter-spacing: 0.02rem;
  color: #7367f0;
}

.navbar-toggle-icon {
  position: absolute;
  top: 30px;
  left: 225px;
  text-decoration: none;
}

.navbar-toggle-icon span {
  font-size: 1.32rem;
  color: #7367f0;
}

.navbar-menu {
  display: flex;
  justify-content: center;
  align-items: center;
  list-style: none;
  margin-top: 37px;
}

.navbar-menu li {
  margin-right: 40px;
}

.navbar-menu a {
  text-decoration: none;
  color: #625f6e;
}

.navbar-menu span {
  position: relative;
}

.navbar-menu span:first-child {
  position: absolute;
  top: 86px;
  left: 27px;
}

.badge {
  width: 20px;
  height: 19px;
  position: absolute;
  left: 200px;
  top: 87px;
  color: #ff9f43;
  background-color: rgba(205, 118, 35, 0.1);
  border: 1px solid rgba(205, 118, 35, 0.02);
  border-radius: 50%;
  font-size: 13px;
  font-weight: bold;
}

.navbar-menu span:last-child {
  position: absolute;
  left: 228px;
  top: 87px;
  font-size: 19px;
}

.dropdown-list {
  list-style-type: circle;
  position: absolute;
  top: 85px;
  left: 54px;
  color: #777;
}

.dropdown-list .list-item {
  position: absolute;
  left: 0;
  top: 50px;
}

.list-item a .list-title {
  left: 0;
  top: 0;
  font-size: 15px;
  letter-spacing: 0.4px;
  margin-left: 12px;
}

.list-item:last-child {
  margin-top: 40px;
}

.apps-pages span {
  position: relative;
  right: 20px;
  bottom: 0;
}

.apps-pages span.apps-title {
  font-weight: 500;
  font-size: 13px;
  color: #a6a4b0;
  position: relative;
  right: 50px;
  top: 130px;
  text-transform: uppercase;
}

.apps-pages .apps-items {
  list-style: none;
  position: absolute;
  top: 280px;
  left: 15px;
}

.apps-pages .item-icons {
  text-decoration: none;
  color: #625f6e;
}
.apps-pages .item-icons span:first-child {
  font-size: 22px;
}

.apps-pages .item-icons span:last-child {
  display: flex;
  justify-content: flex-start;
  position: relative;
  left: 53px;
  bottom: 25px;
}
</style>
