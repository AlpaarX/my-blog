<template>
    
</template>

<script>
export default {
    data() {
        return {
            posts: [
            { id: 1, title: 'Capybaras', body: 'I love capybaras' },
            ],
            title: '',
            body: '',
        }
    },
    methods: {
        createPost() {
            const newPost = {
                id: Date.now(),
                title: this.title,
                body: this.body
            }
            this.posts.push(newPost)
            this.title = ''
            this.body = ''
       },
       deletePost() {
            posts = [...posts, ]
       }
    },
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Noto+Serif+JP:wght@200;300;400;500;600;700;900&family=Roboto:ital,wght@0,100;0,300;0,400;0,500;0,700;0,900;1,100;1,300;1,400;1,500;1,700;1,900&display=swap');
    * {
        box-sizing: border-box;
        margin: 0;
        padding: 0;
        font-family: 'Roboto', sans-serif;
    }
    body {
        background-color: rgb(239, 239, 239);
    }
    .post-list {
        margin: 2rem;
    }
    .post {
        background-color: #ffffff;
        box-shadow: 0 0 10px 0 rgba(0, 0, 0, 0.2);
        border-radius: 10px;
        padding: 1rem;
        margin-bottom: 1rem;
    }
    form {
        background-color: #ffffff;
        box-shadow: 0 0 10px 0 rgba(0, 0, 0, 0.2);
        padding: 1rem;
    }
    .post-input, button {
        width: 100%;
        margin-bottom: 1rem;
        font-size: 1.5rem;
        border-radius: 10px;
        box-shadow: 0 0 10px 0 rgba(0, 0, 0, 0.2);
    }
    .post-input {
        padding: .5rem;
        border: none;
    }
    button {
        border: none;
        padding: .5rem;
        background-color: #4648cb;
        color: white;
    }
    button:active {
        opacity: 0.8;
        box-shadow: none;
        
    }
</style>