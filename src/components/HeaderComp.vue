<template>
<header class="container">
  <!-- LOGO -->
  <div class="head-logo">
    <a href="/">
      
      <img src="../assets/img/dc-logo.png" alt="logo png">

    </a>
  </div>

<!-- NAVIGATORE -->
  <div class="head-nav">

    <nav>

      <ul>

        <li v-for="(link, index) in links" :key="index">
          <a :class="{'active': link.current}" :href="link.url">{{link.text}}</a>
        </li>

      </ul>

    </nav>

  </div>
  

</header>
  
</template>

<script>

export default {
  name: 'HeaderComp',
  data(){
    return{
      links: [
        {
          text: 'Characters',
          url: '#',
          current: false
        },
        {
          text: 'Comics',
          url: '#',
          current: true
        },
        {
          text: 'Movies',
          url: '#',
          current: false
        },
        {
          text: 'Tv',
          url: '#',
          current: false
        },
        {
          text: 'Games',
          url: '#',
          current: false
        },
        {
          text: 'Collectibles',
          url: '#',
          current: false
        },
        {
          text: 'Videos',
          url: '#',
          current: false
        },
        {
          text: 'Fans',
          url: '#',
          current: false
        },
        {
          text: 'News',
          url: '#',
          current: false
        },
        {
          text: 'Shop',
          url: '#',
          current: false
        },
      ]
    }
  }
}
</script>

<style lang="scss" scoped> 
@import '../assets/style/vars.scss';
header{
  height: 120px;
  height: 120px;
  display: flex;
  align-items: center;
}
.head-logo, 
.head-nav{
  width: 50%;
}
.head-logo{

  width: 30%;
}
.head-nav{

  width: auto;
  nav{
    width: 100%;
  }

}

ul{

  display: flex;
  width: 100%;
  justify-content: right;
  margin: 2rem 0;
  font-size: 0.85rem;

  a{
    padding: 20px;
    color: black;
    text-transform: uppercase;
    &:hover,
    &.active{
      border-bottom: 5px solid $blue;
      padding-bottom: 48px;
      border-bottom: 5px solid $blue;
    }
  }
  
}
  
</style>