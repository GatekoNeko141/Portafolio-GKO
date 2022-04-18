<template>
  <div class="content">
    <div class="hvh-100 align-c-c">
      <inicio />
    </div>

    <div class="align-t-c">
      <about />
    </div>

    <div class="hvh-100 align-c-c">
      <portfolio />
    </div>
  </div>
</template>

<script>
import inicio from "../components/content/inicio";
import about from "../components/content/about";
import portfolio from "../components/content/portfolio";
export default {
  layout: "template",
  components: {
    inicio,
    about,
    portfolio
  },
};
</script>

<style scoped>
.content {
  font-family: "Roboto Mono";
  color: #d9ebff;
  letter-spacing: 1.5px;
  word-spacing: -1.8px;
}
</style>
