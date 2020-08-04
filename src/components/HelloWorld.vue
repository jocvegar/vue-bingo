<template>
  <div class="hello page mt-4">
    <div>
      <b-jumbotron
        header="BootstrapVue"
        lead="Bootstrap v4 Components for Vue.js 2"
      >
        <h1>{{ msg }}</h1>
      </b-jumbotron>
    </div>
    <p>
      Are you feeling sad? Just stop and
      <a href="https://be-happy-ok.netlify.app/" target="_blank" rel="noopener">
        Be Happy Ok </a
      >.
    </p>

    <b-container class="bv-example-row">
      <b-row>
        <b-col>
          <b-button class="mx-1" variant="primary">Primary</b-button>
          <b-button class="mx-1" variant="secondary">Secondary</b-button>
          <b-button class="mx-1" variant="success">Success</b-button>
          <b-button class="mx-1" variant="danger">Danger</b-button>
          <b-button class="mx-1" variant="warning">Warning</b-button>
          <b-button class="mx-1" variant="info">Info</b-button>
          <b-button class="mx-1" variant="light">Light</b-button>
          <b-button class="mx-1" variant="dark">Dark</b-button>
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
.page {
  min-height: 842px;
  padding-top: 5px;
  page-break-after: always;
  position: relative;
  margin-left: 2em;
  margin-right: 2em;
  border-bottom: 0.1rem solid #42b983;
}
</style>
