<template>
  <div>
    <LeoMashiro
      @add="sumNum"
      :leomashiro-value="a"
      :value-b="b"
      :value-c="c"
    ></LeoMashiro>
  </div>
</template>

<script>
// 引入组件
import LeoMashiro from "./components/LeoMashiro.vue";
export default {
  // 注册组件
  components: {
    LeoMashiro,
  },
  data() {
    return {
      a: 102,
      b: 130,
      c: 140,
    };
  },
  methods: {
    sumNum() {
      console.log("123");
    },
  },
};
</script>

<style>
</style>
