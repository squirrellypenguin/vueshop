<template>
    <div class="box p-5 mb-4 rounded-3">

        <div id="carouselExampleControls" class="carousel slide" data-bs-ride="carousel">
  <div class="carousel-inner">
    <div class="carousel-item active">
      <img src="https://res.cloudinary.com/doammukzv/image/upload/v1682682860/Art/Halstrom6_zdisrz.jpg" class="d-block w-100" alt="...">
    </div>
    <div class="carousel-item">
      <img src="https://res.cloudinary.com/doammukzv/image/upload/v1682931111/Little_Guys_1_twdlmj.jpg" class="d-block w-100" alt="...">
    </div>
    <div class="carousel-item">
      <img src="https://res.cloudinary.com/doammukzv/image/upload/v1682682859/Art/Halstrom4_a5hsb9.jpg" class="d-block w-100" alt="...">
    </div>
  </div>
  <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleControls" data-bs-slide="prev">
    <span class="carousel-control-prev-icon" aria-hidden="true"></span>
    <span class="visually-hidden">Previous</span>
  </button>
  <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleControls" data-bs-slide="next">
    <span class="carousel-control-next-icon" aria-hidden="true"></span>
    <span class="visually-hidden">Next</span>
  </button>
</div>



        <div class="container-fluid py-5">
    
            <h1 class="display-5 fw-bold"><slot></slot></h1>
            <p class="col-md-8 fs-4 tag">
                A Cooperative Community
            </p>
        </div>
    </div>
</template>