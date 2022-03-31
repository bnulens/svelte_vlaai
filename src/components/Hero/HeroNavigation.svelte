<div class="hero-navigation-wrapper">
  <ul class="hero-navigation">
    <li class="hero-navigation-item" />
    <li class="hero-navigation-item" />
    <li class="hero-navigation-item" />
    <li class="hero-navigation-item" />
  </ul>
</div>

<style lang="scss">
  .hero-navigation-wrapper {
    display: flex;
    flex-direction: column;
    justify-content: flex-end;
    position: relative;
    height: 100%;
    width: 95%;
    margin: 0 auto;

    .hero-navigation {
      display: flex;
      align-items: center;
      justify-content: space-between;
      margin: 0 auto 24px;
      width: clamp(90px, 30%, 220px);

      .hero-navigation-item {
        position: relative;
        display: block;
        width: 12px;
        height: 12px;
        border: 1px solid white;
        border-radius: 50%;

        &:hover {
          cursor: pointer;

          &::after {
            display: block;
            position: absolute;
            content: "";
            top: 50%;
            left: 50%;
            width: 70%;
            height: 70%;
            border: none;
            border-radius: 50%;
            transform: translate(-50%, -50%);
            background-color: white;
          }
        }
      }
    }
  }
</style>
