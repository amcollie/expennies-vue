<script setup>
import Dashboard from './components/Dashboard.vue'
</script>

<template>
  <div class="container">
    <header class="d-flex flex-wrap justify-content-center py-3 mb-4">
      <a href="/" class="d-flex align-items-center mb-3 mb-md-0 me-md-auto text-dark text-decoration-none">
        <img src="./assets/images/logo.png" width="64" height="64" alt="Expennies Logo" />
        <span class="fs-1 fw-bold">Ex<span class="text-primary">pennies</span></span>
      </a>

      <ul class="nav nav-pills align-items-center">
        <li class="nav-item"><a href="#" class="nav-link fw-bold fs-5 active" aria-current="page">Overview</a></li>
        <li class="nav-item"><a href="#" class="nav-link fw-bold fs-5" aria-current="page">Transactions</a></li>
        <li class="nav-item"><a href="#" class="nav-link fw-bold fs-5" aria-current="page">Categories</a></li>
      </ul>
    </header>
    <div class="container">
      <Dashboard />
    </div>
  </div>
</template>

<style lang="scss">
  $primary: #018EFC;

  @import "node_modules/bootstrap/scss/bootstrap.scss";

  * {
    font-family: 'Roboto', sans-serif !important;
  }

  body {
    background-color: #e7ebee;
  }

  .nav-link {
    color: #9aa0a9;

    &.active {
      background-color: inherit !important;
      color: #57585A !important;
    }

    &:hover, &:focus {
      color: #57585A !important;
    }
  }
</style>
