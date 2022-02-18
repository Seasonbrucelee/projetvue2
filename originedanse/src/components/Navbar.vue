<template>
  <div class="hello">
    <div class="home">
  <nav class="navbar navbar-expand-lg navbar-light bg-light">
  <div class="container-fluid">
   <img src="@/assets/logo_texte.png" alt="logo" width="150">
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarSupportedContent">
      <ul class="navbar-nav me-auto mb-2 mb-lg-0">
        <li class="nav-item">
          <a class="nav-link active" aria-current="page" href="#">Accueil</a>
        </li>
        <li class="nav-item dropdown">
          <a class="nav-link dropdown-toggle" href="#" id="navbarDropdown" role="button" data-bs-toggle="dropdown" aria-expanded="false">
          Cours Open
          </a>
          <ul class="dropdown-menu" aria-labelledby="navbarDropdown">
            <li><a class="dropdown-item" href="#">Krump débutant</a></li>
            <li><a class="dropdown-item" href="#">Krump intermédiare</a></li>
            <li><hr class="dropdown-divider"></li>
            <li><a class="dropdown-item" href="#">Événements</a></li>
          </ul>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Professeurs</a>
        </li>

       <li class="nav-item">
          <a class="nav-link" href="#">Formations</a>
        </li>
      </ul>
      <form class="d-flex">
        <input class="form-control me-2" type="search" placeholder="Chercher" aria-label="Search">
        <button class="btn btn-outline-success" type="submit">Chercher</button>
      </form>
    </div>
  </div>
</nav>
  </div>

  </div>
</template>

<script>
export default {
  name: 'Navbar',
  };

</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
