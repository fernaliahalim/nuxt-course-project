<template>
    <div class="admin-post-page">
        <section class="update-form">
            <AdminPostForm :post="loadedPost" />
        </section>
    </div>
</template>

<script>
    import AdminPostForm from '@/components/Admin/AdminPostForm'
    
    export default {
        components: {
            AdminPostForm
        }, data() {
            return {
                loadedPost: {
                    author: 'Fernalia',
                    title: 'My Awesome Post',
                    thumbnailLink: 'https://specials-images.forbesimg.com/imageserve/5f302109ffad89f9130e07db/960x0.jpg?cropX1=0&cropX2=4800&cropY1=243&cropY2=2943',
                    content: 'Super amazing, thanks for that!'
                }
            }
        }
    }
</script>

<style scoped>
    .update-form {
        width: 90%;
        margin: 20px auto;
    }

    @media (min-width: 768px) {
        .update-form {
            width: 500px;
        }
    }
</style>