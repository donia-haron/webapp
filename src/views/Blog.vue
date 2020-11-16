<template>
    <div class="our-blog">
        <h1>{{pageName}}</h1>
        <p>{{pageDescription}}</p>
        <div class="container">
            <div class="row">
                <div class="col-md-8">
                    <div class="posts-area">

                        <BlogPosts v-for="post in posts" :key="post.id" :views="post.views" :title="post.title" :category="post.category" :author="post.author" :date="post.date" :content="post.content"/>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="slidebar" ></div>
                    </div>
                <BlogSidebar/>
                
                </div>
            <div class="alert alert-success alert-dismissible fade show" role="alert">
                learn vue
                <button type="button" class="close" data-dismiss="alert" aria-label="Close">
                    <span aria-hidden="true">&times;</span>
                </button>
            </div>
        </div>
    </div>

</template>


<script>
    import BlogPosts from "@/components/BlogPosts.vue";
    import BlogSidebar from "@/components/BlogSidebar.vue";
    import jsonpost from "../json/BlogPosts.json";


    export default {

        data: function () {
            return {
                pageName: "blog page",
                pageDescription: "this is blog page",
                posts: jsonpost
            };
        },
        name: 'Blog',
        components: {
            BlogPosts,
            BlogSidebar
        }
    };

</script>