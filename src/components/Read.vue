t<template>
  <div>
     <h2>사용자 게시판</h2>
      <div class="container" v-for="(value,index) in data" :key="index">

            <div class="f_wrap">
                <div class="title">{{value.title}}</div>
                <div class="name">{{value.writer}}</div>
              </div>
            <div class="content">{{value.content}}</div>
          </div>
        <button>글쓰기</button>
      </div>

</template>
<script>
  import data from "@/data";
  export default {
    name: 'Read',
    data() {
      return {
        data: data
      };
    }
  };
</script>