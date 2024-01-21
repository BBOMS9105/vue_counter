<script>
export default {
  data() {
    return {
      num: 0
    };
  },
  methods: {
    increasement() {
      this.num++;
    },
    decreasement() {
      this.num--;
    }
  },
};
</script>
<template>
  <h1>{{ num }}</h1>
  <!-- <button v-on:click="increasement">증가</button>
  <button v-on:click="decreasement">감소</button> -->
  <!-- v-on 디렉티브의 축약형 @ -->
  <button @click="increasement">증가</button>
  <button @click="decreasement">감소</button>
</template>