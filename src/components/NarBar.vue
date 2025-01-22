<template>
  
  <nav class="navbar navbar-expand-lg bg-body-tertiary">
      <img alt="Vue logo" class="logo" src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAMwAAADACAMAAAB/Pny7AAAAaVBMVEX///8hISEAAADr6+sODg4KCgoaGhq7u7sdHR0XFxfx8fESEhJbW1v19fVSUlLW1tZMTEyQkJA5OTkuLi7i4uJiYmK0tLSlpaXOzs5ubm7c3NxnZ2fIyMitra1zc3N9fX2FhYVBQUGcnJyDQamwAAADz0lEQVR4nO3Z65aaMBiFYfJBIMhZPCCggPd/kQ0oY4LQUaN2da39/EwReA0DmFoWAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAPyXytrz6jL66jFXm0/s9NjRld9ODxDt0zAM41YZqvuRMFT3cBmZqhL1U3G/n6ZUPpXvJgdLTv1G1euR0Y5RwK5com2hzU+UEeectsrQbhghZcTuR+5QXijbeMOnUqVvldJZvxaKTm5E69J60aoln6mIMvUIMkYOOnqMHBG+FsNmuGstxpFDQazFuNSutJjU7z/2ckx7PY+A88C91MT2XQx/KMb568zMxPiMTurBDGOSy2lwP62qOO+vNzpol+wTMf620mxP6lnNxzBeKRsZxoTOMBnVLtlskvqcEjW2tsETMST3oVOv14UYxsPb/JnFRGK4PLbjIZImW022eCJG/xomlmKY03nviSmHPxN+vB1g+qj5fAxz8vH4ZjHJsDvuLW/xhRjm+9llxCzGHmaG2uVH/zdimKDTMGJ4A8iHPxo6LJ7HUoz7zhj52bQfMYw50vVJ2ZSr2Q3Gh2Zk/zguzUy5slX6Dv8ew6jbmD8018744A+P5cxXe4lhLFeIhYdmrhHa8/C3GMa7wjimWI+vIvJ167C7288Y498MV+ZcjOurqHoqRtbUdWwWY9Xh7T2TKN5PZmeMmfr93YwfHosRY5LTNZ1rFmOVWUfOeAYOPxTav15jXLoJlmJIt30kRqybePwq/OHeahRjRckxpLFHUJdo/zjEyEMefsTBfAzfH/cqT7vhL8S4a69ItYk1i5E2Sf9aNl67Mz8BwkfuZq/cmmWMVcb0zhh50qukueZQexfzuYdmH2NFIb01Zjin07BPkStT8+mH5hBjWSd6d4xlnS819W3kKzMjZSTeHVPn/Q1FKC+e34qxjm5gHmN7yjl4/y7G8tbcNGZzovAnZ9P0+xNMOeIzMfNvd4/GWEXMhVFMIu8j3D/svf5n8+4wfDd+qmzwTMzR0+zUOX8gxiorRxjE1MPzSnBi6baK/eutWf2t9szqTOBoHlmd0WLklRGI12PO46KZ6JeaxP1j5qmYCf/XdbNpjGVn/PWYVS3I1c9AXwM0WQR8IcaK9uS/fgOwzwHdXpvlpaG/UfUxrutOlmeF6waBFuPOcPQYLoe4FjMscbPJgrNnsDwrT7fIfhbO4930jiRjhBCTGCaEq8eIGZOZ4XJIi4mypm2bVnuvlQqajjzNLpOFH85fF33ivzoAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA4GP+ALxdSN3VQ9LwAAAAAElFTkSuQmCC" width="90" height="90" />
  <div class="container-fluid">
    <a class="navbar-brand" href="#">SHEIN(Exam)</a>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarScroll" aria-controls="navbarScroll" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarScroll">
      <ul class="navbar-nav me-auto my-2 my-lg-0 navbar-nav-scroll" style="--bs-scroll-height: 100px;">
        <li class="nav-item">
          <RouterLink class="nav-link active" to="/" aria-current="page">Accueil
          </RouterLink>
        </li>
        <li class="nav-item">
          <RouterLink class="nav-link" to="/about" >Nouveauté</RouterLink>
        </li>
        <li class="nav-item">
          <RouterLink class="nav-link" to="/about" >vetements pour femmes</RouterLink>
        </li>
        <li class="nav-item">
          <RouterLink class="nav-link" to="/about" >Vetements pour hommes</RouterLink>
        </li>
        <li class="nav-item dropdown">
          <a class="nav-link dropdown-toggle" href="#" role="button" data-bs-toggle="dropdown" aria-expanded="false">
            Collection
          </a>
          <ul class="dropdown-menu">
            <li><a class="dropdown-item" href="#">Action</a></li>
            <li><a class="dropdown-item" href="#">Contact</a></li>
            <li><hr class="dropdown-divider"></li>
            <li><a class="dropdown-item" href="#">Best Sellers</a></li>
          </ul>
        </li>
        <li class="nav-item">
          <a class="nav-link disabled" aria-disabled="true">Siting</a>
        </li>
      </ul>
      <form class="d-flex" role="search">
        <input class="form-control me-2" type="search" placeholder="Search" aria-label="Search">
        <button class="btn btn-outline-success" type="submit">Search</button>
      </form>
    </div>
  </div>
</nav>
 </template>
    
  <script >
  import { ref,computed } from "vue";
  const Menu = ref([
    { name: "Home", href: "/home" },
    { name: "Collection", href: "#collection" },
    { name: "What's new", href: "#new" },
    { name: "Best Sellers", href: "#bestsellers" },
    { name: "Gift Ideas", href: "#giftideas" },
    { name: "Contact", href: "#contact" },
  ]);
  
  const scrollToSection = (href) => {
    isMenuOpen.value = false;
    const section = document.querySelector(href);
    if (section) {
      section.scrollIntoView({ behavior: "smooth" });
    }
  };
  </script>