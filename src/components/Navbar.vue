<script setup>
  import Offcanvas from './Offcanvas.vue';
</script>

<template>
  <header class="border-bottom">
    <div class="container-fluid py-2">
      <div class="d-flex align-items-center justify-content-between">

        <div class="d-flex">
          <button class="btn" data-bs-toggle="offcanvas" type="button" data-bs-target="#offcanvas">
            <i class="bi bi-list" style="font-size: 1.5rem;"></i>
          </button>
          <a href="/" class="d-flex align-items-center link-body-emphasis text-decoration-none">
            <img src="../assets/images/logo.png" alt="logo" width="90">
          </a>
        </div>

        <form class="col-5 d-none d-md-flex" role="search">
          <div class="input-group search-bar">
            <input type="text" class="form-control" placeholder="Search" aria-label="Search"
              aria-describedby="basic-addon2">
            <div class="input-group-append">
              <button class="btn btn-outline-secondary text-white px-3 bg-body-tertiary" type="button">
                <i class="bi bi-search"></i>
              </button>
            </div>
          </div>
          <button class="btn btn-dark rounded-5 mx-2 bg-body-tertiary">
            <i class="bi bi-mic"></i>
          </button>
        </form>

        <div class="d-flex">
          <button class="btn btn-dark rounded-5 mx-1 d-none d-md-block">
            <i class="bi bi-upload"></i>
          </button>
          <button class="btn btn-dark rounded-5 mx-1 d-none d-md-block">
            <i class="bi bi-bell"></i>
          </button>
          <button class="btn btn-dark rounded-5 mx-1 d-md-none">
            <i class="bi bi-search"></i>
          </button>
          <div class="dropdown text-end mx-2">
            <a href="#" class="d-block link-body-emphasis text-decoration-none dropdown-toggle"
              data-bs-toggle="dropdown" aria-expanded="false">
              <img src="https://github.com/mdo.png" alt="mdo" width="32" height="32" class="rounded-circle">
            </a>
            <ul class="dropdown-menu text-small">
              <li><a class="dropdown-item" href="#">New project...</a></li>
              <li><a class="dropdown-item" href="#">Settings</a></li>
              <li><a class="dropdown-item" href="#">Profile</a></li>
              <li>
                <hr class="dropdown-divider">
              </li>
              <li><a class="dropdown-item" href="#">Sign out</a></li>
            </ul>
          </div>
        </div>

      </div>
    </div>
  </header>

  <Offcanvas/>

  <nav class="py-2 border-bottom">
    <div class="container d-flex flex-wrap">
      <ul class="nav me-auto">
        <li class="nav-item"><a href="#" class="nav-link link-body-emphasis px-2 active" aria-current="page">Home</a>
        </li>
        <li class="nav-item"><a href="#" class="nav-link link-body-emphasis px-2">Features</a></li>
        <li class="nav-item"><a href="#" class="nav-link link-body-emphasis px-2">Pricing</a></li>
        <li class="nav-item"><a href="#" class="nav-link link-body-emphasis px-2">FAQs</a></li>
        <li class="nav-item"><a href="#" class="nav-link link-body-emphasis px-2">About</a></li>
      </ul>
      <ul class="nav">
        <li class="nav-item"><a href="#" class="nav-link link-body-emphasis px-2">Login</a></li>
        <li class="nav-item"><a href="#" class="nav-link link-body-emphasis px-2">Sign up</a></li>
      </ul>
    </div>
  </nav>


</template>

<style>
.search-bar {
  input {
    border-radius: 50px;
  }

  button {
    border-top-right-radius: 50px;
    border-bottom-right-radius: 50px;
  }
}


</style>