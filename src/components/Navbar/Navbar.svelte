<script>
  import NavbarItem from "./NavbarItem.svelte";
</script>

<div class="component-wrapper" id="home">
  <div class="navbar-wrapper">
    <NavbarItem link={"#home"} title={"Home"} />
    <nav class="main-navbar">
      <NavbarItem link={"#about"} title={"About"} />
      <NavbarItem link={"#context"} title={"Context"} />
      <NavbarItem link={"#guide"} title={"Guide"} />
      <NavbarItem link={"#contact"} title={"Contact"} />
    </nav>
  </div>
</div>

<style lang="scss">
  .component-wrapper {
    position: relative;
    width: 100%;
    height: 100%;

    .navbar-wrapper {
      display: flex;
      justify-content: space-between;
      align-items: center;
      width: 100%;
      height: 40px;

      .main-navbar {
        display: flex;
        justify-content: space-between;
      }
    }

    &:after {
      display: block;
      content: "";
      position: absolute;
      top: 0;
      left: 50%;
      width: 100vw;
      height: 40px;
      background-color: black;
      transform: translate(-50%);
      z-index: -10;
    }
  }
</style>
