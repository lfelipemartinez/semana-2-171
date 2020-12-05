<template>
  <nav
    class="navbar navbar-expand-sm navbar-dark font-weight-bold justify-content-start bg-dark"
  >
    <!-- nav logo -->
    <a class="navbar-brand" href="#">
      <img src="images/logo.png" class="img" alt="Logo" height="50px" />
    </a>
    <!-- boton collapse-->
    <button
      class="navbar-toggler"
      type="button"
      data-toggle="collapse"
      data-target="#collapsibleNavbar"
    >
      <span class="navbar-toggler-icon"></span>
    </button>
    <!--fin del boton collapse-->
    <!-- fin del logo -->
    <!--navbar list-->
    <div
      class="collapse navbar-collapse justify-content-end"
      id="collapsibleNavbar"
    >
      <ul class="navbar-nav">
        <li class="nav-item"><a class="nav-link active" href="#">Inicio</a></li>
        <li class="nav-item">
          <a class="nav-link" href="#services">Servicios</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#news">Noticias</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#team">Miembros</a>
        </li>
      </ul>
    </div>
    <!-- fin del navbar list-->
  </nav>
</template>

<script>
export default {
  name: "PageHeader",
};
</script>