<template>
    <div class="admin-new-post-page">
        <section class="new-post-form">
           <AdminPostForm/>
        </section>
    </div>
</template>
<script>
import AdminPostForm from '@/components/Admin/AdminPostForm'

export default {
    components: {
        AdminPostForm
    },
    data(){
        return {
            editedPost:{
                author :'',
                title :'',
                thumbnailLink :'',
                content :'',

            }
        }
    },
    methods: {
        onSave() {
            console.log(this.editedPost)
        },
        onCancel(){
            this.$router.push('/admin')
        }
    }
}
</script>

