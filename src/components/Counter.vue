<template>
  <div class="headerStyle">
    <h1>{{i}}</h1>
    <button v-on:click="increase(1)">Try increase</button>
    <br />
    <br />
    <button v-on:click="decrease(1)">Try decrease</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      i: 0
    };
  },
  methods: {
    increase: function(x) {
      this.i = this.i + x;
    },

    decrease: function(x) {
      this.i -= x;
    }
  }
};
</script>