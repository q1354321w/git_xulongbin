<template>
<div>
    <MyBlog v-for="blog in blogs" :key="blog.id" :title="blog.title"></MyBlog>
    </div>
    
    
</template>
<script type="text/ecmascript-6">
import MyBlog from "./components/MyBlog";
export default {
    data(){
        return{
            blogs:[
                {id:1,title:'one'},
                {id:2,title:'twoo'},
                {id:3,title:'three'}
            ]
        }
    },
    components:{
        MyBlog,
    }
}
</script>
<style scoped>

</style>

