<template>
  <div class="headerStyle">
    <header>
      <h1>{{ msg }}</h1>
    </header>
  </div>
</template>

<script>
export default {
  data() {
    return {
      msg: "Singapore attractions list"
    };
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
header {
  background: rgb(122, 63, 100);
  padding: 10px;
  border-style: solid;
  border-color: black;
  border-width: 2px;
}
h1 {
  color: rgb(175, 175, 100);
}
</style>