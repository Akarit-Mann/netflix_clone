<template>
  <div class="navbar ">
    <div class="navLogo">
      <img src="../assets/neflix_logo.png" alt="">
    </div>
    <div>
      <button class="btn ">Sign In</button>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style>

  .navbar{
    width: 100%;
    padding: 0 20px !important;
    display: flex;
  }
  .navbar button{
    background-color: #E50914;
    color: #fff;
    padding: 5px 15px;
    margin-right: 20px;
  }
  .navbar .navLogo{
    width: 200px;
  }
  .navbar .navLogo img{
    width: 100%;
  }
</style>