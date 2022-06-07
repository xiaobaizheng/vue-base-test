<template>
  <!-- 这里就是你的html标签，这里要注意一个问题，要在 package.json 里面看一下你使用的vue版本是好多的，如果3.0一下，template这个下面只能像现在这样包裹在一个div里面，如果是3.0及以上就随便了-->
  <div class="hello">
    <h2>
      这里说明一下，如果你在components文件下面新建了一个xxx.vue的文件，那么你需要去注册路由，在router文件夹下面
    </h2>
    <p>例如：</p>
    <p>我在components文件下面新建了test.vue</p>
    <p>
      然后找到src/router/index.js注入你的路由，怎么注入呢？详情找到这个文件去看
    </p>
    <router-link to="/test">点我就可以跳转test页面了</router-link>
    <p>当然，如果你想深入学习，我建议你还是看下vue的文档，这样能更好的上手操作</p>
    <a href="https://cn.vuejs.org/v2/guide/index.html" target="_blank">点我跳转vue2.0文档</a>
    <a href="https://v3.cn.vuejs.org/guide/introduction.html" target="_blank">点我跳转vue3.0文档</a>
  </div>
</template>

<script>
// 这里就是你写的js数据等交互的地方
export default {
  name: "HelloWorld",
  data() {
    return {
      msg: "Welcome to Your Vue.js App"
    };
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
/* 这里就是你的css样式 */
h1,
h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
