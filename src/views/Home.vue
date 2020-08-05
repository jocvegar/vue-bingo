<template>
  <div>
    <div class="home">
      <!-- <img alt="Vue logo" src="../assets/logo.png" /> -->
      <HelloWorld msg="Come Home!" id="Card0" />
      <HelloWorld msg="Come Home!" id="Card1" />
      <HelloWorld msg="Come Home!" id="Card2" />
      <HelloWorld msg="Come Home!" id="Card3" />
      <HelloWorld msg="Come Home!" id="Card4" />
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
