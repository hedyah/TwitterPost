<template>
    <div>
        <h3>{{postTitle}}</h3>
        <p>{{postContent}}</p>
        <p>{{postDate}}</p>
    </div>
</template>

<script>

    export default {
        name: "TwitterPost",
        props: {
            postTitle: String,
            postContent : String,
            postDate: String,
            id: Number
        },
    }
</script>

<style  scoped>
*{
    border: 2px rgb(0, 0, 0) solid;
    background-color: blanchedalmond;
}
div{
    font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
    font-size: 22px;
    
}
</style>