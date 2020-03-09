<template>
  <div>
    <counter></counter>
    <ul>
      <li v-for="item in itemsList" v-bind:key="item.name">
        <h2>{{item.name}}</h2>
        <counter></counter>

        <img v-bind:src="item.image" />
      </li>
    </ul>
  </div>
</template>


<script>
import Counter from "./Counter.vue";
export default {
  components: {
    counter: Counter
  },

  data() {
    return {
      itemsList: [
        { name: "f1", image: "./assets/f1.jpg", show: false },
        { name: "ion", image: "/assets/ion.jpg", show: false },
        { name: "mbs", image: "/assets/mbs.jpg", show: false },
        { name: "flyer", image: "/assets/flyer.jpg", show: false },
        {
          name: "gardensbythebay",
          image: "/assets/gardensbythebay.jpg",
          show: false
        },
        { name: "nus", image: "/assets/nus.jpg", show: false }
      ]
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
  color: ivory;
}
h2 {
  text-align: center;
}
#itemsList {
  width: 100%;
  max-width: 120px;
  margin: 30px auto;
  padding: 0 5px;
  box-sizing: border-box;
}
ul {
  display: flex;
  flex-wrap: wrap;
  list-style-type: none;
  padding: 0;
}
li {
  flex-grow: 1;
  flex-basis: 300px;
  text-align: center;
  padding: 10px;
  border: 1px solid #222;
  margin: 10px;
}

img {
  max-width: 150px;
}
</style>