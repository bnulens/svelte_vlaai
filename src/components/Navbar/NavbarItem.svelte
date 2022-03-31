<script>
  export let link;
  export let title;
</script>

<a class="main-navbar-item" href={link}>{title}</a>

<style lang="scss">
  .main-navbar-item {
    color: white;
    font-size: clamp(8px, 2vw, 14px);
    margin: 0 12px;
  }
</style>
