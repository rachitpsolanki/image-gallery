<template>
    <div class="gallery">
        <div class="title">
            <h2>Image Gallery</h2>
            <p>Some description about this awesome image gallery made using vue.js</p>
        <div>
        </div>
            <img class="image-item" src="../assets/logo.png" height="200" width="200"  v-for="i in 10" :key='i'/>
        </div>
    </div>
</template>
<script>
export default {
    name:'Gallery'
}
</script>
<style>
.gallery .image-item{
margin: 5px;
}
.gallery .title *{
    text-align: center;
}
.gallery img{
    transition: ease-in-out;
    transition-duration: 0.2s;
}
.gallery img:hover{
    transform: scale(1.2);
}
</style>
