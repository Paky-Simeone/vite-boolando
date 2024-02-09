<script>
import Appheader from './components/Appheader.vue';
import Appmain from './components/Appmain.vue';
import Appfooter from './components/Appfooter.vue';
export default{
  data(){
    return{

    }
  },
  components: { Appheader, Appmain, Appfooter }
};


</script>

<template>
<Appheader></Appheader>
<Appmain></Appmain>
<Appfooter></Appfooter>
</template>

<style lang="scss">
@use './styles/general.scss';
</style>
