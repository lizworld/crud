<template>
  <div>
    <h2>상세페이지</h2>
        <div class="container">
            <div class="f_wrap">
                <div class="title">{{data.title}}</div>
                <div class="writer">{{data.writer}}</div>
              </div>
            <div class="content">{{data.content}}</div>

          </div>
  </div>
</template>
<script>
  import data from "@/data";
  export default {
    name: 'Detail',
    data() {
      const index = this.$route.params.contentId
      return {
        data: data[index],

      }
    }
  }
</script>