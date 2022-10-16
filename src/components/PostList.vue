<template>
  <div class="post-list">
        <div class="post" v-for="post in posts">
            <p style="user-select: none; text-align: end;">❌</p>
            <p><strong>Название:</strong> {{post.title}}</p>
            <p><strong>Описание1:</strong> {{post.body}}</p>
        </div>
    </div>
</template>

<script>
  export default {
    
  }
</script>

<style scoped>

</style>