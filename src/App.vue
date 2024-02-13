<script>
import {store} from './store';
import axios from 'axios';
import Appheader from './components/Appheader.vue';
import Appmain from './components/Appmain.vue';
import Appfooter from './components/Appfooter.vue';
export default{
  data(){
    return{
      products : [],
    }
  },
  components: { Appheader, Appmain, Appfooter }
};


</script>

<template>
<Appheader></Appheader>
<div v-for="product in products">{{ product.name }}</div>
<Appmain></Appmain>
<Appfooter></Appfooter>
</template>

<style lang="scss">
@use './styles/general.scss';
</style>
