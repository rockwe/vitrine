<template>
<div class="container">
	<div class="row bg-danger mb-5 p-3">
		<div class="col"><p class=" p-1  border-dark text-center text-white"><font-awesome-icon :icon="['fas', 'house']" /> Telecharge l'app et <span> et beneficiez de reduction</span></p></div>
		<div class=" col"><p class=" p-2 border-dark text-center text-white"> <FontAwesomeIcon :icon="faDragon" />Affiliation</p></div>
		<div class=" col "><p class=" p-2  border-dark text-center text-white"> 15% de reduction <span> et beneficiez de reduction</span> </p></div>
		<div class="col "><p class=" p-2  border-dark text-center text-white"> Carte cadeau</p></div>

	</div>
	<div class="row ">
		<div class="col"><p class=" p-2  border-dark text-center "> Carte cadeau</p></div>
		<div class="col">
			<div id="carouselExampleIndicators" class="carousel slide">
  <div class="carousel-indicators">
    <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="0" class="active" aria-current="true" aria-label="Slide 1"></button>
    <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="1" aria-label="Slide 2"></button>
    <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="2" aria-label="Slide 3"></button>
  </div>
  <div class="carousel-inner">
    <div class="carousel-item active">
      <img src="@/assets/product01D.webp" class="d-block w-100" alt="...">
    </div>
    <div class="carousel-item">
      <img src="@/assets/product02D.webp" class="d-block w-100" alt="...">
    </div>
    <div class="carousel-item">
      <img src="@/assets/product03D.webp" class="d-block w-100" alt="...">
    </div>
  </div>
  <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide="prev">
    <span class="carousel-control-prev-icon" aria-hidden="true"></span>
    <span class="visually-hidden">Previous</span>
  </button>
  <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide="next">
    <span class="carousel-control-next-icon" aria-hidden="true"></span>
    <span class="visually-hidden">Next</span>
  </button>
</div>
		</div>
		<div class="col"><p class=" p-2  border-dark text-center "> Carte cadeau</p></div>
	</div>
</div>
</template>

<script>

</script>

<style >

span{
	 font-family: Times, sans-serif;
  font-size: 70%
}
</style>