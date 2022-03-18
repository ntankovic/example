<template>
  <div class="about">
    <h1>This is an about page {{ id }}</h1>
    {{ $route.params.id }}
    <router-view />
  </div>
</template>
<script>
export default {
  name: "AboutPage",
  props: ["id"],
  mounted() {
    console.log(this.$route);
    console.log(this);
  },
};
</script>
