<template>
  <div>
     <h2>글쓰기</h2>
        <div class="container">
      <input v-model="writer" type="text" placeholder="글쓴이">
      <input v-model="title" type="text" placeholder="제목">
      <textarea v-model="content" cols="30" rows="10" placeholder="내용을 입력하세요"></textarea>
      <button @click="write">글쓰기</button>
         
    </div>
  </div>
</template>
<script>
  import data from '@/data'
  export default {
    name: 'Create',
    data() {
      return {
        data: data,
        writer: '',
        title: '',
        content: ''
      }
    },
    methods: {
      write() {
        this.data.push({
          writer: this.writer,
          title: this.title,
          content: this.content
        })
        this.$router.push({
          path: '/'
        })
      }
    },
  }
</script>