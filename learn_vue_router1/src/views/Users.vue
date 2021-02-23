<template>
  <div>
    <h1>Users</h1>
    <router-link to="/users/1">ユーザー１</router-link>
    <router-link to="/users/2">ユーザー2</router-link>
    <hr>
    <h1>User No.{{ id }}</h1>
   <router-link :to=
   "'/users/' + (Number(id) + 1) + '/profile'"
   >次</router-link>
    <router-view></router-view>
  </div>
</template>

<script>
export default {
  props: ["id"]
};
</script>
