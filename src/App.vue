<script>
export default {
  data() {
    return {
      str: 'Hello Vue.js',
      num: 0,
      bool: true,
      undi: undefined,
      nul: null,
      arr: [10],
      obj: {
        name: 'Hong',
        age: 20
      }
    };
  },
  methods: {
    dataChange() {
      this.str = 'Hi Vue.js';
      this.num = 10;
      this.bool = false;
      this.undi = 'undefined';
      this.nul = 'null';
      this.arr.push(20);
      this.obj = {
        name: 'Kim',
        age: 30
      };
    }
  },
};
</script>
<template>
  <h1>{{ str }}</h1>
  <h1>{{ num }}</h1>
  <h1>{{ bool }}</h1>
  <h1>{{ undi === undefined ? "undefined" : "not undefined"}}</h1>
  <h1>{{ nul === null ? "null" : "not null" }}</h1>
  <h1>{{ arr }}</h1>
  <h1>{{ obj }}</h1>
  <button @click="dataChange">변경</button>
</template>