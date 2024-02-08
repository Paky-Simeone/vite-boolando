<script>
export default{
    data(){
        return{
            images: [
                {
                    image: '../assets/img/1.webp',
                    imageHover: '../assets/img/1b.webp'
                },
                {
                    image: '../assets/img/2.webp',
                    imageHover: '../assets/img/2b.webp'
                },
                {
                    image: '../assets/img/3.webp',
                    imageHover: '../assets/img/3b.webp'
                },
                {
                    image: '../assets/img/4.webp',
                    imageHover: '../assets/img/4b.webp'
                },
                {
                    image: '../assets/img/5.webp',
                    imageHover: '../assets/img/5b.webp'
                },
                {
                    image: '../assets/img/6.webp',
                    imageHover: '../assets/img/6b.webp'
                },
            ],
        }
    },
    methods: {
        generateURL(path) {
         return new URL(path, import.meta.url).href;
        }
    }
}
</script>

<template>
<div v-for="immagine in images" >
    <img :src="generateURL(immagine.image)" alt="image" />
    <img :src="generateURL(immagine.imageHover)" alt="imageHover" />
</div>
</template>

<style>

</style>