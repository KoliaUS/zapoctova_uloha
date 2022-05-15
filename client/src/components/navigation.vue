<template>
  <header>
    <div class="px-3 py-2 bg-dark text-white">
      <div class="container">
        <div class="d-flex flex-wrap align-items-center justify-content-center justify-content-lg-start">
          <a href="/" class="d-flex align-items-center my-2 my-lg-0 me-lg-auto text-white text-decoration-none ">
            <em class="bi-book"></em>
          </a>

          <ul class="nav col-12 col-lg-auto my-2 justify-content-center my-md-0 text-small">
            <li>
            <router-link class="nav-link text-secondary" to="/rent">
              <em class="bi-archive d-block mx-auto mb-1 w-25 h-25" ></em>
              neco
            </router-link>
            </li>
            <li>
              <router-link class="nav-link text-secondary" to="/about">
                <em class="bi-archive d-block mx-auto mb-1 w-25 h-25" ></em>
                necll
              </router-link>
            </li>
            <li>
              <a href="#" class="nav-link text-white">
                <svg class="bi d-block mx-auto mb-1" width="24" height="24"><use xlink:href="#table"/></svg>
                Orders
              </a>
            </li>
            <li>
              <a href="#" class="nav-link text-white">
                <svg class="bi d-block mx-auto mb-1" width="24" height="24"><use xlink:href="#grid"/></svg>
                Products
              </a>
            </li>
            <li>
              <a href="#" class="nav-link text-white">
                <svg class="bi d-block mx-auto mb-1" width="24" height="24"><use xlink:href="#people-circle"/></svg>
                Customers
              </a>
            </li>
          </ul>
        </div>
      </div>
    </div>

  </header>

</template>

<script>
export default {
  name: "navigation"
}
</script>

<style scoped>

</style>