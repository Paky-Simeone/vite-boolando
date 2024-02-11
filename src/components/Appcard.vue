<script>
export default{
    props: {
        img: String,
        // newimg: String,
        title: String,
    },
};
</script>

<template>
    
    <div class="card">
        <img :src="img" :alt="title">
        <!-- <img :src="newimg" :alt="title"> -->
        <p class="heart">&hearts;</p>
        <p class="sale">-50%</p>
        <p class="sostenibilità">Sostenibilità</p>
    </div>
     
</template>

<style lang="scss" scoped>

</style>