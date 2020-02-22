<template>
  <main>
    <section>
      <h1>🧛‍♂️ Mis repos en Github...💩</h1>
      <div class="projects" v-for="project in githubProjects" :key="project.id">
        <h3>
          <a :href="project.html_url">{{ project.name }}</a>
        </h3>
        <p class="stars">🌟 {{ project.stargazers_count }}</p>
        <p>{{ project.homepage }}</p>
        <p>{{ project.description }}</p>
      </div>
    </section>
    <aside>
      <h3>
        Hola soy Israel alias
        <code>"iukones"</code>
      </h3>
      <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Ea error impedit odio libero laudantium dolorum fugit deserunt incidunt quod eum? Aspernatur cum quas ullam! Omnis vel numquam ex dolorum saepe.</p>
    </aside>
  </main>
</template>

<script>
import { mapState } from "vuex";

export default {
  computed: {
    ...mapState(["githubProjects"])
  }
  //se crea plugin para meter el dispatch del store...
  // mounted() {
  //   this.$store.dispatch("getGithubProjects");
  // }
};
</script>

<style lang="scss" scoped>
main {
  width: 80vw;
  margin: 2% 8%;
  display: grid;
  grid-template-columns: 2fr 1fr;
  grid-template-rows: 1fr;
  grid-column-gap: 50px;
  grid-row-gap: 0px;
}

section {
  background-color: white;
  color: black;
  padding: 30px;
  grid-area: 1 / 1 / 2 / 2;
  h1 {
    margin-bottom: 1.5rem;
  }
  a {
    color: black;
  }
}
aside {
  grid-area: 1 / 2 / 2 / 3;
  h3 {
    margin-bottom: 1.5rem;
  }
}
.projects {
  padding-bottom: 1rem;
  margin-bottom: 1.5rem;
  border-bottom: 1px dashed #8494a8;
}
.stars {
  color: orangered;
}
</style>