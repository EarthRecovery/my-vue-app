<template>
  <div class="hello">
    <div id="background">
      <div id="block">
        <h1>{{ headline }}</h1>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String,
  },
  data() {
    return {
      headline: "Klein Kaslana",
      img1: require("../assets/img1.jpg"),
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
#background {
  background: url("../assets/bg.jpg") no-repeat;
  background-color: rgba(255, 255, 255, 0.5);
  background-position: center;
  height: 100%;
  width: 100%;
  background-size: cover;
  position: absolute;
  display: flex;
  justify-content: center;
  align-items: center;
}

#block {
  background: #ffffff;
  background-color: rgba(255, 255, 255, 0.9);
  height: 100%;
  width: 75%;
  position: absolute;
  justify-content: center;
}

h1 {
  font-size: 100px;
  font-family: "Times New Roman", Times, serif;
  color: #000000;
  text-align: center;
  margin: 0;
  padding: 0;
}
</style>
