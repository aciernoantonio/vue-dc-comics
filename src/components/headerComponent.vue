<template>
    
    <header>

    <nav>

      <div class="container">

      <div class="d-flex center navbar">

        <div>
          <img src="@/assets/dc-logo.png" alt="">
        </div>
        <div class="navLink">

          <a href="">CHARACTERS</a>
          <a class="active" href="">COMICS</a>
          <a href="">MOVIES</a>
          <a href="">TV</a>
          <a href="">GAMES</a>
          <a href="">COLLECTIBLES</a>
          <a href="">VIDEOS</a>
          <a href="">FAMS</a>
          <a href="">NEWS</a>
          <a href="">SHOP</a>

        </div>

      </div>

    </div>

    </nav>

  </header>
    
</template>

<script>

export default {
  name: "app",
  components: {
    
  }
}
</script>


<style lang="scss" scoped>

@import "@/assets/scss/style";

    nav{

  a{
    margin: 0 0.75rem;
    text-decoration: none;
    color: black;
  }

  img{
    width: 75%;
    padding: 1rem 0;
  }

  .navLink {
    font-size: 0.75rem;
    font-weight: bold;
  }

  .navbar{
    justify-content: space-around;
  }

  .active{
    color: #0282F9;
    border-bottom: 7px solid #0282F9;
    padding-bottom: 2.7rem
  }

}

</style>