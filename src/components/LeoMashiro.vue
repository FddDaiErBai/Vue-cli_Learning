<template>
  <div>
    <h1>我是LeoMashiro{{a}}</h1>
    <button @click="add">按我加1</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      a:100
    }
  },
  methods: {
    add(){
      this.a++
    }
  },
};
</script>

<style>
</style>