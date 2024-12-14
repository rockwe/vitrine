<template>
<div id="carouselExampleAutoplaying" class="carousel slide" data-bs-ride="carousel">
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
  <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleAutoplaying" data-bs-slide="prev">
    <span class="carousel-control-prev-icon" aria-hidden="true"></span>
    <span class="visually-hidden">Previous</span>
  </button>
  <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleAutoplaying" data-bs-slide="next">
    <span class="carousel-control-next-icon" aria-hidden="true"></span>
    <span class="visually-hidden">Next</span>
  </button>
</div>
<div class="global">
		<section class="top-articles">
			<div class="div">
				<h2 class="category-title">First steps</h2>
				<ul class="list-articles">
					<li class="article">
						<li><router-link to="/premiersPas">What's Netflix ?</router-link></li>
					</li>
					<li class="article">
						<a href="">How to pay for my Netflix subscription ?</a>
					</li>
				</ul>
			</div>
			<div class="div">
				<h2 class="category-title">Cannot read</h2>
				<ul class="list-articles">
					<li class="article">
						<a href="/mdp">I forgot my Netflix username or password</a>
					</li>

				</ul>
			</div>
			<div class=" div">
				<h2 class="category-title">Quick links</h2>
				<ul class="list-articles">
					<li class="article">
						<a href="#"> Reset password </a>
					</li>
				
					<li class="article">
						<a href="">Update Email </a>
					</li>

					<li class="article">
						<a href="#">Request movies or TV shows </a>
					</li>
				</ul>
			</div>


			<div class=" div">
				<h2 class="category-title">Watch Netflix</h2>
				<ul class="list-articles">
					<li class="article">
						<a href="#"> idée1 </a>
					</li>
				
					<li class="article">
						<a href="">idée2 </a>
					</li>

					<li class="article">
						<a href="#">idée3 </a>
					</li>
				</ul>
			</div>
		</section>
	</div>
<footer class="iq-footer">
    <div class="container-fluid">
      <div class="row">
        <div class="col-lg-6">
          <ul class="list-inline mb-0">
            <slot name="left"></slot>
          </ul>
        </div>
        <div class="col-lg-6 text-right">
          <slot name="right"></slot>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>

</script>

<style>
</style>