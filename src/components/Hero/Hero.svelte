<script>
  import Gallery from "./Gallery.svelte";
  import HeroNavigation from "./HeroNavigation.svelte";
</script>

<div class="component-wrapper" id="hero">
  <div class="hero-wrapper">
    <Gallery />
    <HeroNavigation />
  </div>
</div>

<style lang="scss">
  .component-wrapper {
    position: relative;
    width: 100vw;
    height: 65vh;
    transform: translate(-50%);
    margin-left: 50%;

    .hero-wrapper {
      width: 100%;
      height: 100%;
      background-color: hsla(120, 100%, 25%, 0.521);
    }
  }
</style>
