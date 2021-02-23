<template>
  <div style="width: 700px; margin: auto; padding-top: 50px;">
    <nav>
      <router-link
      to="/"
      active-class="link--active"
      class="link"
      exact
      >Home</router-link>
      <router-link
      to="/users"
      active-class="link--active"
      exact
      class="link"
      >Users</router-link>
    </nav>
    <router-view></router-view>
  </div>
</template>

<style scoped>
  .link {
    margin-right: 15px;
  }
  .link--active {
    font-size: 20px;
  }
</style>
