<template>
  <div>
    <theOneComment
      v-for="(item, index) in commentsArr"
      :info="item"
      :key="index"
    ></theOneComment>
  </div>
</template>

<script>
// 引入组件
import theOneComment from "./components/theOneComment.vue";
// 引入文件
import comments from "./comments.js";

export default {
  // 注册组件
  components: {
    theOneComment,
  },
  data() {
    return {
      commentsArr: comments,
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
