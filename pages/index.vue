<template>
  <main>
    <div class="backgrounds">
      <app-masthead />
    </div>

    <div class="headings">
      <h1>
        Hola mundo
        <br />yo amo los tacos. 🌮
      </h1>
      <p>Por favor come muchos tacos. 🌮</p>
    </div>

    <div class="links">
      <p>Sigueme para mas tutoriales</p>
    </div>

    <div class="nextpage">Página de prueba</div>
  </main>
</template>

<script>
import appMasthead from "~/components/appMasthead.vue";

export default {
  components: {
    appMasthead
  }
};
</script>

<style lang="scss" scoped>
main {
  width: 100vw;
  height: calc(100vh - 100px);
  display: grid;
  grid-template-columns: repeat(2, 100px) repeat(3, 1fr);
  grid-template-rows: repeat(3, 1fr) 50px 100px;
  grid-column-gap: 0px;
  grid-row-gap: 0px;
}

.backgrounds {
  grid-area: 1 / 3 / 5 / 6;
}
.headings {
  grid-area: 2 / 2 / 3 / 6;
}
.links {
  padding: 30px;
  grid-area: 5 / 1 / 6 / 5;
}
.nextpage {
  background-color: #eee;
  color: black;
  padding: 30px;
  grid-area: 4 / 5 / 6 / 6;
}
</style>
