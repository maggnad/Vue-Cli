<template>
  <header class="header">
    <div class="container">
      <div class="header__wrap">
        <router-link to="/" class="logo"> lopo </router-link>
        <ul class="menu">
          <li class="menu__list">
            <router-link to="/" class="menu__list-link">About</router-link>
          </li>
          <li class="menu__list">
            <router-link to="/" class="menu__list-link">Menu</router-link>
          </li>
          <li class="menu__list">
            <router-link to="/" class="menu__list-link">Active</router-link>
          </li>
          <li class="menu__list">
            <router-link to="/" class="menu__list-link">Contacts</router-link>
          </li>
        </ul>
      </div>
    </div>
  </header>
</template>



<script>
export default {
  name: "HeaderView",
};
</script>
<style lang="scss">
.header {
  background: #a50598;
  color: aqua;
  padding: 20px 0;
}
.header__wrap {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.logo {
  color: aqua;
  font-size: 20px;
}
.menu {
  display: flex;
  align-items: center;
  gap: 30px;
}
.menu__list-link {
  color: aqua;
  font-family: Arial, Helvetica, sans-serif;
  font-size: 20px;
}
@media screen and (max-width: 991px) {
  .header__wrap {
    flex-direction: column;
    justify-content: center;
    align-items: center;
    gap: 20px;
  }
}
</style>