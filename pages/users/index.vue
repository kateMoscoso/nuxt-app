<template>
<div>
<Header />
<p> Please enter and id</p>
</div>
</template>
<script>

export default {
    data(){
       return {
           userId:''
       }
    },
    methods: {
        onLoadUser(){
            this.$router.push('/users/'+this.userId)
        }
    },
  layout: 'users'
}
</script>