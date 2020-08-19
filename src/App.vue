<template>
  <div id="app">
    <img class="rounded-circle" src="./assets/1.jpg" width="20%" />
    <HelloWorld msg="Nonog_Narlux" />
    <hr />
    <div class="row">
      <div class="col">
        <img class="rounded border border-dark" src="./assets/5.jpg" width="80%" />
        <br />
        <br />
        <coun />
      </div>
      <div class="col">
        <img class="rounded border border-dark" src="./assets/3.jpg" width="80%" />
        <br />
        <br />
        <coun />
      </div>
      <div class="col">
        <img class="rounded border border-dark" src="./assets/6.jpg" width="80%" />
        <br />
        <br />
        <coun />
      </div>
    </div>
    <div class="row">
      <div class="col">
        <fonts />
        <hr />
        <div class="row-12">
          ชื่อ-นามสกุล
          <input type="text" v-model="name" />
          รหัส นศ.
          <input type="number" v-model="code" />
          GPA
          <input type="number" v-model="gpa" step="0.1" />
          <br />
          <br />
        </div>
        <div class="row-12">แสดง:ชื่อ {{name}} รหัส นศ.{{code}} GPA {{gpa}}</div>
        <br />
        <br />
      </div>
    </div>
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";
import coun from "./components/coun.vue";
import fonts from "./components/fonts.vue";
export default {
  name: "App",
  components: {
    HelloWorld,
    coun,
    fonts,
  },
  data: function () {
    return {
      total: 0,
      name: "",
      code: "",
      gpa: 0.1,
    };
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
