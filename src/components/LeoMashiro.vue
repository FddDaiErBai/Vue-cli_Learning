<template>
  <div>
    <h1>
      我是LeoMashiro 我接收到的父组件的值是：{{ leomashiroValue }}
      {{ valueB }} {{ valueC }}
    </h1> 
    <button @click="add">按我加1</button>
  </div>
</template>

<script>
export default {
  // 罗列父组件传进来的属性值
  props: {
    leomashiroValue:Number,
    valueB: Number,
    valueC: Number,
  },
  methods:{
    add(){
      this.$emit("add")
    }
  }
}
</script>

<style>
</style>