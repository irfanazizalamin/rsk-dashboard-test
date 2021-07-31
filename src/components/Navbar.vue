<template>
  <nav class="navbar navbar-expand-lg navbar-light">
    <div class="container">
      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <a class="navbar-brand" href="#">
          <img src="../assets/img/icons/rsk-logo.svg" alt="rsk-logo" height="60">
        </a>
        <ul class="navbar-nav me-auto mb-2 mb-lg-0">
          <li class="nav-item">
            <router-link class="nav-link" to="/">
              <button
                id="nav-member" type="button"
                class="btn"
                onclick="blur()"
              >
                Kelas
              </button>
            </router-link>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" to="/">
              <button
                id="nav-member" type="button"
                class="btn"
                onclick="blur()"
              >
                Lowongan
              </button>
            </router-link>
          </li>
        </ul>

        <form class="mx-auto d-flex">
          <input
            class="form-control me-2"
            type="search"
            placeholder="Cari Kelas"
            aria-label="Search"
          >
        </form>

        <ul class="navbar-nav ml-auto mb-2 mb-lg-0">
          <li class="nav-item">
            <router-link class="nav-link" to="/">
              <button
                id="nav-member" type="button"
                class="btn"
                onclick="blur()"
              >
                Kawan Cuan
              </button>
            </router-link>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" to="/">
              <button type="button" class="btn btn-primary">Daftar / Masuk</button>
            </router-link>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: 'Navbar',
};
</script>

<style>
.navbar {
  background-color: #ffc709;
  box-shadow: 0 4px 2px -2px rgba(0,0,0,.2);
}

#nav-member {
  outline: none;
  padding: 4px 8px;
  font-size: 18px;
  font-weight: 500;
}

#nav-member:hover {
  background: rgba(0, 0, 0, 0.1);
}
</style>
