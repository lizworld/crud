<template>
  <div id="app">
    <router-view />
  </div>
</template>

<script>
  export default {
    name: 'App'
  }
</script>

<style>
  @import url("https://cdn.jsdelivr.net/gh/orioncactus/pretendard@v1.3.6/dist/web/static/pretendard.css");

  * {
    margin: 0;
    padding: 0;
    font-family: -apple-system, BlinkMacSystemFont, "Apple SD Gothic Neo", "Pretendard Variable", Pretendard, Roboto, "Noto Sans KR", "Segoe UI", "Malgun Gothic", "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", sans-serif;
  }

  #app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
  }

  h2 {
    background-color: #2c3e50;
    color: #fff;
    line-height: 50px;
  }

  button {
    border: 0;
    padding: 0 20px;
    line-height: 2;
    font-weight: 600;
    background-color: #2c3e50;
    color: #fff;
    margin: 10px 5px;
    display: inline-block;
    cursor: pointer;
  }

  input,
  textarea {
    border: 0;
    width: 100%;
    display: block;
    background-color: #f4faff;
    line-height: 2;
    text-indent: 20px;
    margin-bottom: 10px
  }

  .container {
    margin: 20px 30px
  }

  .f_wrap {
    display: flex;
    flex-wrap: wrap;
    background-color: rgb(241, 241, 241);
    padding: 10px 20px;
    text-align: left;
  }

  .title {
    flex-grow: 9;
    font-weight: 999;
  }

  .writer {
    flex-grow: 1;
  }

  .content {
    padding: 10px 20px;
    background-color: aliceblue;
    min-height: 10vw;
  }
</style>