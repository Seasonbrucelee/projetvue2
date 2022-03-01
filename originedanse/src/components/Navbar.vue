<template>
  <div class="hello">
    <div class="home">
  <nav class="navbar navbar-expand-lg navbar-light">
  <div class="container-fluid">
   <img src="@/assets/logo_texte.png" alt="logo" width="150">
    <button class="navbar-toggler" type="button" style= "color:#b4351c;" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon" style= "color:#b4351c;"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarSupportedContent">
      <ul class="navbar-nav me-auto mb-2 mb-lg-0">
        <li class="nav-item">
          <a class="nav-link active" style= "color:#b4351c;" aria-current="page" href="#">Accueil</a>
        </li>
        <li class="nav-item dropdown">
          <a class="nav-link dropdown-toggle" style= "color:#b4351c;" href="#" id="navbarDropdown" role="button" data-bs-toggle="dropdown" aria-expanded="false">
          Cours Open
          </a>
          <ul class="dropdown-menu" style="background-color: #031472;" aria-labelledby="navbarDropdown">
            <li><a class="dropdown-item" style= "color:#b4351c;" href="#">Krump débutant</a></li>
            <li><a class="dropdown-item" style= "color:#b4351c;" href="#">Krump intermédiare</a></li>
            <li><hr class="dropdown-divider"></li>
            <li><a class="dropdown-item" style= "color:#b4351c;" href="#">Événements</a></li>
          </ul>
        </li>
        <li class="nav-item">
          <a class="nav-link" style= "color:#b4351c;" href="#">Professeurs</a>
        </li>

       <li class="nav-item">
          <a class="nav-link" style= "color:#b4351c;"  href="#">Formations</a>
        </li>
      </ul>
      <form class="d-flex">
        <input class="form-control me-2" style= "color:#b4351c;" type="search" placeholder="Chercher" aria-label="Search">
        <button class="btn btn-outline-success" style= "color:#b4351c;"   type="submit">Chercher</button>
      </form>
    </div>
  </div>
</nav>
  </div>

</template>

<script>
export default {
  name: 'Navbar',
  };
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.navbar{
 background-color: #031472;
}
a{
  color:#b4351c;
}

.dropdown-item{
color:#b4351c;
}
.dropdown-item{
  font-size: 30px;
}
</style>
