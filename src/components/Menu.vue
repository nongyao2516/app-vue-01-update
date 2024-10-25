<template>

  <div id="nav" v-if="!isLoginPage">

<header class="p-3 text-bg-primary">
    <div class="container">
      <div class="d-flex flex-wrap align-items-center justify-content-center justify-content-lg-start">
        <a href="/" class="d-flex align-items-center mb-2 mb-lg-0 text-white text-decoration-none">
          <svg class="bi me-2" width="40" height="32" role="img" aria-label="Bootstrap"><use xlink:href="#bootstrap"></use></svg>
        </a>

        <ul class="nav col-12 col-lg-auto me-lg-auto mb-2 justify-content-center mb-md-0">
          <li><a href="/" class="nav-link px-2 text-white">Home</a></li>
          <li><a href="/product" class="nav-link px-2 text-white">Product</a></li>
          <li><a href="/member" class="nav-link px-2 text-white">Member</a></li>
          <li><a href="/about" class="nav-link px-2 text-white">About</a></li>
        
        
        </ul>

        <form class="col-12 col-lg-auto mb-3 mb-lg-0 me-lg-3" role="search">
          <input type="search" class="form-control form-control-dark text-bg-white" placeholder="Search..." aria-label="Search">
        </form>

        <div class="text-end">
        <a href="/login"> <button type="button" class="btn btn-outline-light me-2">Login</button> </a>
          <button type="button" class="btn btn-warning">Sign-up</button>
        </div>
      </div>
    </div>
  </header>
</div>



  </template>
  
  <script>
import { computed } from 'vue'
import { useRoute } from 'vue-router'

  export default {
      neme: 'Menu',
      setup() {
    const route = useRoute()
    
    // ตรวจสอบว่า route ปัจจุบันเป็น 'Login' หรือไม่
    const isLoginPage = computed(() => route.name === 'Login')
    
    return { isLoginPage }
  }

  }
  </script>
  
  <style>

</style>