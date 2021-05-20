<template>

<div class="jumbotron">

  <div class="container">


    <div>

      <ul>

        <li>

          <img src="../assets/img/buy-comics-digital-comics.png" alt="carta">

          <a href="#">digital comics</a>

        </li>

        <li>

          <img src="../assets/img/buy-comics-merchandise.png" alt="maglietta">

          <a href="#">dc merchandise</a>

        </li>

        <li>

          <img src="../assets/img/buy-comics-subscriptions.png" alt="subscript">

          <a href="#">subscription</a>

        </li>

        <li>

          <img src="../assets/img/buy-comics-shop-locator.png" alt="shop">

          <a href="#">comic shop locator</a>

        </li>

        <li>

          <img src="../assets/img/buy-dc-power-visa.svg" alt="power">

          <a href="#">dc power visa</a>

        </li>

      </ul>

    </div>


  </div>
</div>

</template>

<script>
export default {
  name: 'SubMain'
}
</script>

<style lang="scss" scoped>

@import '../assets/style/vars.scss';

.jumbotron{
  height: 150px;
  background-color: #0C7CEC;

    .container{
      
      ul{

        display: flex;
        

        li{

          display: flex;
          align-items: center;
          /* padding: 50px; */
          padding-top: 50px;
          padding-right: 30px;
          padding-left: 50px;

          a{
            color: white;
            padding-left: 10px;
            text-transform: uppercase;
            font-size: 13px;
          }
        }
      }

    }
}

img{
  width: 40px;
  height: 50px;
}
</style>