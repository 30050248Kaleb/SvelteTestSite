<nav class="navbar navbar-expand-lg navbar-light bg-light">
    <div class="container-fluid">
      <a class:active={$page.url.pathname === '/'} class="navbar-brand" href="/">Svelte Site</a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNavDropdown" aria-controls="navbarNavDropdown" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNavDropdown">
        <ul class="navbar-nav">
          <li class="nav-item">
            <a class:active={$page.url.pathname === '/'} class="nav-link" aria-current="page" href="/">Home</a>
          </li>
          <li class="nav-item">
            <a class:active={$page.url.pathname === '/about'} class="nav-link" href="/about">About</a>
          </li>
          <li class="nav-item">
            <a class:active={$page.url.pathname === '/superheroes/dc'} class="nav-link" href="/superheroes/dc">DC Superheroes</a>
          </li>
          <li class="nav-item">
            <a class:active={$page.url.pathname === '/superheroes/marvel'} class="nav-link" href="/superheroes/marvel">Marvel Superheroes</a>
          </li>
        </ul>
      </div>
    </div>
  </nav>

  <script>
    import { page } from '$app/stores';
  </script>