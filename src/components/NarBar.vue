<template>
  
  <nav class="navbar navbar-expand-lg bg-body-tertiary">
      <img alt="Vue logo" class="logo" src="@/assets/18.jpg" width="90" height="90" />
  <div class="container-fluid">
    <a class="navbar-brand" href="#">Navbar scroll</a>
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
          <RouterLink class="nav-link" to="/about" >About</RouterLink>
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