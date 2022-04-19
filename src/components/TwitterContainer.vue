<template>
    <div>
        <h1>{{userinput}}</h1>

        <TwitterPost v-for="post in posts"
        :key="post.id"
        :postDate="post.postDate"
        :postTitle="post.postTitle"
        :postContent="post.postContent"
        :id="post.id"
        />
        
    </div>
</template>

<script>
import TwitterPost from './TwitterPost.vue'

    export default {
    components: { TwitterPost },
        name: "TwitterContainer",
        data() {
            return {
                userinput : "",
                posts: [
                    {
                    id : 1,
                    postDate : "April 16 2022",
                    postTitle : "FunnyTweets101",
                    postContent : " I'll never forget a week after quarantine started I sneezed in the grocery store and a man two aisles over yelled AW HELL NAWL."
                    },
                    {
                    id: 2,
                    postDate : "March 22 2022",
                    postTitle : "RelatableTweets233",
                    postContent : " Ur on wordle, I'm on my 30th attempt to guess my own password"
                    }
                    
                    
                ]
            }
        },
    }
</script>

<style scoped>
*{
    background-color: burlywood;
}
</style>