<template>

  <div>
    <div>
      <img :src="card.thumb" :alt="card.series" />
    </div>

    <div class="title">
      <h5>{{ card.series }}</h5>
    </div>
  </div>

  
</template>

<script>
export default {
  name: "Volume",

  props: {
    card: Object,
  },
};
</script>

<style lang="scss" scoped>
div {
  flex-basis: calc(100% / 6);
  img {
    width: 140px;
    height: 140px;
    margin-top: 50px;
    color: white;
  }
  h5 {
    margin-bottom: 30px;
    color: white;
    
  }
}
</style>
