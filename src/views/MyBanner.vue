<template>
  <div id="carouselExampleIndicators" class="carousel slide" data-bs-ride="carousel">
    <div class="carousel-indicators">
      <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="0" class="active" aria-current="true" aria-label="Slide 1"></button>
      <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="1" aria-label="Slide 2"></button>
      <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="2" aria-label="Slide 3"></button>
      <button type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide-to="3" aria-label="Slide 4"></button>
    </div>
    <div class="carousel-inner">
      <div class="carousel-item active">
        <img src="../.././src/images/banner.png" class="d-block w-100" alt="...">
      </div>
      <div class="carousel-item">
        <img src="../.././src/images/banner.png" class="d-block w-100" alt="...">
      </div>
      <div class="carousel-item">
        <img src="../.././src/images/banner.png" class="d-block w-100" alt="...">
      </div>
      <div class="carousel-item">
        <img src="../.././src/images/banner.png" class="d-block w-100" alt="...">
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "MyBanner"
}
</script>

<style scoped>
.carousel-indicators button{
  width: 6px;
  height: 6px;
  border-radius: 50%;
}
.carousel-indicators{
  bottom: -15px;
}
.carousel-indicators .active{
  background-color: #ff1605;
}
</style>