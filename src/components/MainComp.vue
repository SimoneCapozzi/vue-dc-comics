<template>
  
  <main>

    <div class="jumbotron ">
        
    <button class="btn-center"><h3>current series</h3></button>

    </div>


    <div class="container">

      

      <VolumeDc 
      v-for="(volume, index) in volumi"
      :key="index"
      :card="volume"
      />

      <button class="btn-dw">load more</button>

    </div>

    

  </main>

</template>

<script>

import volumi from "@/assets/data/dc-comics.js";

import VolumeDc from "@/components/VolumeDc.vue"

export default { 
  name: 'MainComp',

  components:{
    VolumeDc
  },

  data(){

    return{
      volumi
    }
  },

  mounted(){
    console.log(volumi);
  }
}
</script>

<style lang="scss" scoped>

@import '@/assets/style/vars.scss';


  
main{
  
  min-height: 300px;
  background-color: #1C1C1C;

  .jumbotron{
    
    height: 400px;
    width: 100%;
    background-image: url(../assets/img/jumbotron.jpg);
    background-size: cover;
  }

  .btn-center{
    
    padding: 5px 40px;
    margin-bottom: 20px;
    color: white;
    background: $blue;
    border: 0;
    text-transform: uppercase;
    margin-left: 300px;
    margin-top: 386px;
  }

  div{
    
    flex-wrap: wrap;
  }
  
  .btn-dw{
    margin: auto;
    padding: 5px 40px;
    margin-bottom: 20px;
    color: white;
    background: $blue;
    border: 0;
    text-transform: uppercase;
  }


}

</style>