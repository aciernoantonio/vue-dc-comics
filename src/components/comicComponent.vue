<template>
    

    <div class="comic">

        <img :src="img" alt="">

        <div>{{title}}</div>
                    
    </div>


</template>

<script>
export default {
    name: "comicItem",
    props: {
        img: String,
        title: String
    }
}
</script>

<style lang="scss" scoped>

.comic{
    text-align: center;
    width: calc(100% / 6);
    padding: 1rem;

    img{
        width: 150px;
        height: 150px;
    }
}


</style>