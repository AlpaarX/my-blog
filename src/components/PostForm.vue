<template>
  <form @submit.prevent>
        <input 
            v-bind:value="title"
            @input="event => title = event.target.value" 
            class="post-input" 
            type="text" 
            placeholder="Название">
        <input 
            v-bind:value="body" 
            @input="event => body = event.target.value" 
            class="post-input" 
            type="text" 
            placeholder="Описание">
        <button 
            @click="createPost">Создать
        </button>
    </form>
</template>

<script>
  export default {
    
  }
</script>

<style lang="scss" scoped>

</style>
