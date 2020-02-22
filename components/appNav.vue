<template>
  <div>
    <ul>
      <li>
        <nuxt-link exact to="/">Inicio</nuxt-link>
      </li>
      <li>
        <nuxt-link to="/test-page">Repositorios</nuxt-link>
      </li>
    </ul>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
div {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 100vw;
  height: 100px;
  ul {
    padding-left: 0;
    li {
      display: inline-block;
      margin-right: 30px;
    }
  }
}
</style>