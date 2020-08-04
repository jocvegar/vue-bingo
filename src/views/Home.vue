<template>
  <div>
    <div class="home">
      <!-- <img alt="Vue logo" src="../assets/logo.png" /> -->
      <HelloWorld msg="Come Home!" />
      <HelloWorld msg="Come Home!" />
      <HelloWorld msg="Come Home!" />
      <HelloWorld msg="Come Home!" />
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue";

export default {
  name: "Home",
  components: {
    HelloWorld
  }
};
</script>
