<template>
  <div class="about">
    <h1>This is an about page</h1>
    <router-link to="/about1">about1</router-link>
    <router-link to="/about2">about2</router-link>
    <router-view></router-view>
  </div>
</template>
<script>
export default {
  data() {
    return {};
  },
  watch: {
    $route(to, from) {
      console.log(from.path); //从哪来
      console.log(to.path); //到哪去
    },
  },
};
</script>