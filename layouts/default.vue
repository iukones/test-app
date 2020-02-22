<template>
  <div>
    <app-nav />
    <nuxt />
  </div>
</template>

<script>
import appNav from "~/components/appNav.vue";

export default {
  components: {
    appNav
  }
};
</script>

<style>
html {
  font-family: "Montserrat";
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
  background: #0b0d17;
  color: #eeeeee;
}

a,
a:visited,
a:active {
  color: white;
  text-decoration: none;
}

*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0;
}
h1,
h2,
h3,
h4,
h5,
h6 {
  font-family: "Krona One";
}
</style>
