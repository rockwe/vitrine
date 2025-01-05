<template>
  <div class="container text-center mt-5">
    <h1 class="display-4">Feel <span class="text-success">Healthy</span> and <span class="text-success">Energetic</span> With Our Vitamins</h1>
    <p class="lead mt-3">
      Our mission is to make you healthy and happy. For this, we use only natural and high-quality ingredients necessary to achieve an extraordinary effect.
    </p>
    <div class="d-flex justify-content-center mt-4">
      <div class="badge bg-secondary me-2">Supplements</div>
      <div class="badge bg-secondary me-2">Fast and Timely Delivery</div>
      <div class="badge bg-secondary">Free Shipping from $30!</div>
    </div>
    <!-- Image principale -->
    <img
      src="https://via.placeholder.com/800x400" 
      alt="Healthy Lifestyle"
      class="img-fluid mt-5"
    />
    <h2 class="mt-5">Popular Categories</h2>
    <!-- Liste des catégories avec images en ligne -->
    <div class="row mt-4">
      <div class="col-md-3" v-for="category in categories" :key="category.id">
        <div class="card">
          <img :src="category.image" class="card-img-top" :alt="category.title" />
          <div class="card-body">
            <h5 class="card-title">{{ category.title }}</h5>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Accueil",
  data() {
    return {
      categories: [
        {
          id: 1,
          title: "Allergy Relief",
          image: "https://images.unsplash.com/photo-1515378960530-7c0da6231fb1",
        },
        {
          id: 2,
          title: "Anxiety",
          image: "https://images.unsplash.com/photo-1494790108377-be9c29b29330",
        },
        {
          id: 3,
          title: "Depression",
          image: "https://images.unsplash.com/photo-1529626455594-4ff0802cfb7e",
        },
        {
          id: 4,
          title: "Eye & Vision",
          image: "https://images.unsplash.com/photo-1503023345310-bd7c1de61c7d",
        },
      ],
    };
  },
};
</script>

<style scoped>
.text-success {
  font-weight: bold;
}
.card-img-top {
  height: 200px;
  object-fit: cover;
}
</style>
