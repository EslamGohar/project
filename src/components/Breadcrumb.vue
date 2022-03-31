<template>
  <div class="breadcrumb">
    <h2 class="title">Shop</h2>

    <div class="breadcrumb-content">
      <ul class="breadcrumb-items">
        <li>
          <a href="#">
            <span class="material-icons-outlined"> home </span>
          </a>
        </li>
        <li><span class="material-icons-outlined"> navigate_next </span></li>
        <li><a href="#" class="">ECommerce</a></li>
        <li><span class="material-icons-outlined"> navigate_next </span></li>
        <li>Shop</li>
      </ul>
    </div>
  </div>

  <div class="settings">
    <div class="dropdown">
      <button class="dropbtn">
        <span class="material-icons-outlined"> settings </span>
      </button>
      <div class="dropdown-content">
        <a href="#">
          <span class="material-icons-outlined"> task </span>
          <span>Todo</span>
        </a>
        <a href="#">
          <span class="material-icons-outlined"> chat_bubble_outline </span>
          <span>Chat</span>
        </a>
        <a href="#">
          <span class="material-icons-outlined"> email </span>
          <span>Email</span>
        </a>

        <a href="#">
          <span class="material-icons-outlined">calendar_today</span>
          <span>Calender</span>
        </a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "breadcrumb-component",
};
</script>

<style scoped>
.breadcrumb {
  display: flex;
  justify-content: center;
  align-items: center;

  position: absolute;
  top: 110px;
  left: 290px;
}

.title {
  font-weight: 500;
  color: #636363;
  border-right: 1px solid #d6dce1;
  padding-right: 1rem;
}

.breadcrumb-items {
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 0.3rem 0.7rem;
  list-style: none;
}

.breadcrumb-items li {
  padding-right: 1px;
  font-size: 14px;
}

.breadcrumb-items a {
  text-decoration: none;
  color: #7367f0;
  font-size: 14px;
}

.breadcrumb-items span {
  font-size: 20px;
  color: #636363;
}

.breadcrumb-items a span:first-child {
  color: #7367f0;
}

.settings {
  display: flex;
  justify-content: flex-end;
}

.dropdown {
  position: absolute;
  top: 112px;
  right: 35px;
}

.dropbtn {
  background-color: #7367f0;
  color: #fff;
  padding: 11px;
  border: none;
  border-radius: 5px;
  cursor: pointer;
}

.dropbtn span {
  font-size: 18px;
}

.dropdown-content {
  display: none;
  position: absolute;
  right: 5%;
  margin-top: 8px;
  background-color: #fff;
  min-width: 160px;
  box-shadow: 0px 8px 16px 0px rgba(0, 0, 0, 0.05);
  border-radius: 5px;
  z-index: 1;
}

.dropdown-content a {
  font-size: 14px;
  color: #636363;
  padding: 11px 5px;
  text-decoration: none;
  display: flex;
  justify-content: flex-start;
  align-items: center;
}

.dropdown-content a span {
  font-size: 15.5px;
  padding-left: 12px;
}

.dropdown-content a:hover {
  background-color: #f1f1f1;
  color: #7367f0;
}

.dropdown:hover .dropdown-content {
  display: block;
}

.dropdown:hover .dropbtn {
  box-shadow: 0 8px 25px -8px #7367f0;
}
</style>
