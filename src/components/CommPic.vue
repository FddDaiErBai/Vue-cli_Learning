<template>
  <div>
    <img
      v-for="(item, index) in imgArr"
      :key="index"
      :src="item.imgUrl"
      @click="changeImg(index)"
      alt=""
    />
    <p class="cur">
      <img :src="imgArr[idx].imgUrl" alt="" />
    </p>
  </div>
</template>

<script>
export default {
  props: ["imgArr"],
  data() {
    return {
      idx: 0,
    };
  },
  methods: {
    changeImg(idx) {
      this.idx = idx;
    },
  },
};
</script>

<style scoped>
img {
  width: 60px;
  margin-right: 10px;
  cursor: pointer;
}
.cur img {
  width: 300px;
}
</style>