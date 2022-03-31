<template>
  <nav class="wrapper">
    <div class="wrapper-icons">
      <div class="left-icons">
        <a href="#"
          ><span class="material-icons-outlined">calendar_today</span></a
        >
        <a href="#"
          ><span class="material-icons-outlined">chat_bubble_outline</span></a
        >
        <a href="#"><span class="material-icons-outlined">mail</span></a>
        <a href="#"><span class="material-icons-outlined">add_task</span></a>
        <a href="#"><span class="material-icons-outlined">star_border</span></a>
      </div>

      <div class="right-icons">
        <ul>
          <div class="options">
            <li>
              <a href="#">
                <span class="material-icons material-icons-outlined">
                  flag
                </span>
                <span class="text">English</span>
              </a>
            </li>
            <li>
              <a href="#"
                ><span class="material-icons-outlined">dark_mode</span></a
              >
            </li>
            <li>
              <a href="#"
                ><span class="material-icons-outlined">search</span></a
              >
            </li>
            <li>
              <a href="#">
                <span class="material-icons-outlined">shopping_cart</span>
                <span class="cart-badge">5</span>
              </a>
            </li>
            <li style="margin-left: -20px">
              <a href="#">
                <span class="material-icons-outlined">notifications</span>
                <span class="notification-badge">6</span>
              </a>
            </li>
          </div>
          <li class="profile-info">
            <a href="#">
              <div class="temp">
                <img
                  src="https://www.pngitem.com/pimgs/m/206-2067982_thinking-boy-clipart-and-cliparts-for-free-transparent.png"
                  alt="avatar"
                  class="img-circle-small"
                />
                <p class="user-name">John Doe</p>
                <span class="user-role">admin</span>
                <span class="status topRight"></span>
              </div>
            </a>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: "navgation-component",
};
</script>

<style scoped>
.wrapper {
  display: flex;
  justify-content: center;
  align-items: center;
}
.wrapper-icons {
  position: fixed;
  top: 18px;
  left: 290px;
  border-radius: 5px;
  background-color: #fff;
  width: 76%;
  height: 63px;
  box-shadow: 0 4px 24px 0 rgb(34 41 47 / 10%);
  z-index: 999;
}

.left-icons {
  display: flex;
  justify-content: center;
  align-items: center;
  position: relative;
  top: 18px;
  right: 40%;
}

.left-icons a {
  text-decoration: none;
  color: #6e6b7b;
}

.left-icons a:last-child {
  color: #ff9f43;
}

.left-icons span {
  padding-left: 12px;
}

.right-icons {
  display: flex;
  align-items: center;
  justify-content: flex-end;
}

.options {
  display: flex;
  align-items: center;
  justify-content: center;
  position: fixed;
  top: 37px;
  right: 177px;
}

.right-icons ul {
  list-style: none;
}

.right-icons a {
  text-decoration: none;
  display: flex;
  margin-left: 15px;
  color: #6e6b7b;
}

.right-icons span.text {
  padding-top: 3px;
  padding-left: 4px;
  font-size: 14px;
}

.right-icons .cart-badge {
  width: 19px;
  height: 19px;
  position: relative;
  right: 15px;
  bottom: 9px;
  color: #fff;
  background-color: #7367f0;
  border: 1px solid #7367f0;
  border-radius: 50%;
  font-size: 11px;
  font-weight: bold;
}

.right-icons .notification-badge {
  width: 19px;
  height: 19px;
  position: relative;
  right: 15px;
  bottom: 9px;
  color: #fff;
  background-color: #ea5455;
  border: 1px solid #ea5455;
  border-radius: 50%;
  font-size: 11px;
  font-weight: bold;
}

.right-icons .profile-info {
  color: #6e6b7b;
  text-align: right;
  position: relative;
  bottom: 17px;
  margin-right: 10px;
}

.right-icons .user-name {
  position: relative;
  right: 54px;
  bottom: 42px;
  font-size: 14px;
  font-weight: 600;
  letter-spacing: 0.5px;
}

.user-role {
  font-size: 12px;
  position: relative;
  right: 54px;
  bottom: 46px;
}

.img-circle-small {
  width: 42px;
  height: 42px;
  border-radius: 50%;
}

.status {
  width: 11px;
  height: 11px;
  border-radius: 50%;
  border: 1px solid #fff;
  margin-bottom: 2px;
  background-color: rgb(24, 216, 24);
  position: absolute;
}

.temp {
  position: relative;
  top: 0;
  right: 10px;
}

.topRight {
  top: 30px;
  right: 0;
}
</style>
