<template>
  <div>
    <h1>
      我是LeoMashiro 我接收到的父组件的值是：{{ leomashiroValue }}
      {{ valueB }} {{ valueC }}
    </h1>
  </div>
</template>

<script>
export default {
  // 罗列父组件传进来的属性值
  props: {
    leomashiroValue: {
      type: Number,
      // 数据的校验
      validator: function (value) {
        return value > 50;
      },
    },
    valueB: Number,
    valueC: Number,
  },
};
</script>

<style>
</style>