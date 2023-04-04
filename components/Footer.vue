<template>
  <footer>
    <div v-for="link in linkList" :key="link.title">
      <a :href="link.url">{{ link.title }}</a>
    </div>
  </footer>
</template>

<script>
// フッターに表示するリンクのリスト
const linkList = [
  {
    title: 'github',
    url: 'https://github.com/YutakaNagai'
  },
]

export default {
  data() {
    return {
      linkList,
    }
  }
}
</script>

<style scoped>
footer {
  width: 100%;
  background-color: rgb(220, 220, 220);
  text-align: center;
  padding: 30px 0;
  position: absolute;/*←絶対位置*/
  bottom: 0; /*下に固定*/
}
</style>