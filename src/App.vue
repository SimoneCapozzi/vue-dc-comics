<template>
  <div id="app">

    <Header-comp />

    <Main-comp />

    <SubMain />

    <Footer-comp />

    <VolumeDc />


  </div>
</template>

<script>

import HeaderComp from '@/components/HeaderComp.vue'

import MainComp from '@/components/MainComp.vue'

import SubMain from '@/components/SubMain.vue'

import FooterComp from '@/components/FooterComp.vue'

import VolumeDc from '@/components/VolumeDc.vue'

export default {
  name: 'App',

  components: {

    HeaderComp,
    MainComp,
    SubMain,
    FooterComp,
    VolumeDc
  }
}
</script>


<style lang="scss">

*{
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}

@import './assets/style/general.scss';
@import './assets/style/utilities.scss';

ul{
  list-style: none;
}

a{
  text-decoration: none;
}

.container{
  display: flex;
  width: 65%;
  margin: 0 auto;
}
</style>
