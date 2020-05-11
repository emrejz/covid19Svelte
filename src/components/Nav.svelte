<script>
  // export let segment;
  let show = false;
  function toggleNavbar() {
    show = !show;
  }
</script>

<style>
  .showNavbar {
    display: block;
  }
</style>

<nav class="navbar navbar-expand-lg navbar-dark bg-dark">
  <a class="navbar-brand" href="/">Navbar</a>
  <button class="navbar-toggler" type="button" on:click={toggleNavbar}>
    <span class="navbar-toggler-icon" />
  </button>

  <div class="collapse navbar-collapse" class:showNavbar={show} id="navbarNav">
    <ul class="navbar-nav">
      <li class="nav-item active">
        <a class="nav-link" href="/">
          Home
          <span class="sr-only">(current)</span>
        </a>
      </li>
      <li class="nav-item">
        <a class="nav-link" href="/features">Features</a>
      </li>
      <li class="nav-item">
        <a class="nav-link" href="/pricing">Pricing</a>
      </li>
      <li class="nav-item">
        <a
          class="nav-link disabled"
          href="/disabled"
          tabindex="-1"
          aria-disabled="true">
          Disabled
        </a>
      </li>
    </ul>
  </div>
</nav>
