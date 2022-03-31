<script>
  import Navbar from "./Navbar/Navbar.svelte";
  import Hero from "./Hero/Hero.svelte";
</script>

<div class="app-container">
  <Navbar />
  <Hero />
</div>

<style lang="scss">
  .app-container {
    display: flex;
    flex-direction: column;
    position: relative;
    height: 100%;
    width: 100%;
    max-width: 95%;
    margin: 0 auto;
  }

  @media only screen and (min-width: 768px) {
    .app-container {
      max-width: 1080px;
    }
  }
</style>
