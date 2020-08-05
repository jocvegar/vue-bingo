<template>
  <div :id="id" class="page mt-4">
    <b-container class="bv-example-row bg-danger text-white pt-2 pb-3 rounded">
      <b-row class="my-3 font-weight-bold py-5 h2 border-bottom">
        <b-col>B</b-col>
        <b-col>I</b-col>
        <b-col>N</b-col>
        <b-col>G</b-col>
        <b-col>O</b-col>
      </b-row>
      <b-row class="my-3 py-3 h5 border-bottom">
        <b-col id="B1" class="border-right"></b-col>
        <b-col id="I1" class="border-right"></b-col>
        <b-col id="N1" class="border-right"></b-col>
        <b-col id="G1" class="border-right"></b-col>
        <b-col id="O1"></b-col>
      </b-row>
      <b-row class="my-3 py-3 h5 border-bottom">
        <b-col id="B2" class="border-right"></b-col>
        <b-col id="I2" class="border-right"></b-col>
        <b-col id="N2" class="border-right"></b-col>
        <b-col id="G2" class="border-right"></b-col>
        <b-col id="O2"></b-col>
      </b-row>
      <b-row class="my-3 py-3 h5 border-bottom">
        <b-col id="B3" class="border-right"></b-col>
        <b-col id="I3" class="border-right"></b-col>
        <b-col id="N3" class="border-right">FREE</b-col>
        <b-col id="G3" class="border-right"></b-col>
        <b-col id="O3"></b-col>
      </b-row>
      <b-row class="my-3 py-3 h5 border-bottom">
        <b-col id="B4" class="border-right"></b-col>
        <b-col id="I4" class="border-right"></b-col>
        <b-col id="N4" class="border-right"></b-col>
        <b-col id="G4" class="border-right"></b-col>
        <b-col id="O4"></b-col>
      </b-row>
      <b-row class="my-3 py-3 h5">
        <b-col id="B5" class="border-right"></b-col>
        <b-col id="I5" class="border-right"></b-col>
        <b-col id="N5" class="border-right"></b-col>
        <b-col id="G5" class="border-right"></b-col>
        <b-col id="O5"></b-col>
      </b-row>
    </b-container>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String,
    id: String
  },
  mounted: function() {
    let arrayB = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15];
    let arrayI = [16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 30];
    let arrayN = [31, 31, 32, 33, 34, 35, 36, 37, 38, 39, 40, 41, 42, 43, 45];
    let arrayG = [46, 47, 48, 49, 50, 51, 52, 53, 54, 55, 56, 57, 58, 59, 60];
    let arrayO = [61, 61, 62, 63, 64, 65, 66, 67, 68, 69, 70, 71, 72, 73, 75];

    const shuffledB = arrayB.sort(() => Math.random() - 0.5).slice(0, 5);
    const shuffledI = arrayI.sort(() => Math.random() - 0.5).slice(0, 5);
    const shuffledN = arrayN.sort(() => Math.random() - 0.5).slice(0, 5);
    const shuffledG = arrayG.sort(() => Math.random() - 0.5).slice(0, 5);
    const shuffledO = arrayO.sort(() => Math.random() - 0.5).slice(0, 5);

    for (let i = 1; i <= shuffledB.length; i++) {
      document.querySelector(`#${this.id} #B${i}`).innerText = shuffledB[i - 1];
    }

    for (let i = 1; i <= shuffledI.length; i++) {
      document.querySelector(`#${this.id} #I${i}`).innerText = shuffledI[i - 1];
    }

    for (let i = 1; i <= shuffledN.length; i++) {
      if (i == 3) {
        document.querySelector(`#${this.id} #N${i}`).innerText = "FREE";
      } else {
        document.querySelector(`#${this.id} #N${i}`).innerText =
          shuffledN[i - 1];
      }
    }

    for (let i = 1; i <= shuffledG.length; i++) {
      document.querySelector(`#${this.id} #G${i}`).innerText = shuffledG[i - 1];
    }

    for (let i = 1; i <= shuffledO.length; i++) {
      document.querySelector(`#${this.id} #O${i}`).innerText = shuffledO[i - 1];
    }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.page {
  min-height: 850px;
  padding-top: 5px;
  page-break-after: always;
  position: relative;
  margin-left: 2em;
  margin-right: 2em;
}
</style>
