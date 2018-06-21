<template>
  <div>
    <nav class="navbar navbar-dark bg-dark navbar-expand-lg">
      <a class="navbar-brand" href="#">Shoptime</a>
      <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNavAltMarkup" aria-controls="navbarNavAltMarkup" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNavAltMarkup">
        <div class="navbar-nav">
          <a class="nav-item nav-link active" href="#">HOME</a>
          <a class="nav-item nav-link" href="#">ORDERS</a>
          <a class="nav-item nav-link" href="#">PRODUCT</a>
        </div>
        <div class="navbar-nav ml-auto">
          <a class="nav-item nav-link ml-auto" href="#">ADMIN</a>
        </div>
      </div>
    </nav>
    <nuxt/>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
.navbar-brand {
  padding: 21px 2px 21px 40px;
}

.navbar-expand-lg {
  .nav-link {
    padding: 21px 20px;
  }

  .nav-link.active {
    border-bottom: 4px solid white;
  }
}
</style>
