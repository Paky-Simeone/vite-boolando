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
        
    </div>
</template>

<style lang="scss" scoped>

</style>