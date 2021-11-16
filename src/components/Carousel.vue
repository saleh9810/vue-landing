<template>
  <div
    id="carouselExampleIndicators"
    class="carousel slide"
    data-bs-ride="carousel"
  >
    <ol class="carousel-indicators">
      <li
        data-bs-target="#carouselExampleIndicators"
        data-bs-slide-to="0"
        class="active"
      ></li>
      <li data-bs-target="#carouselExampleIndicators" data-bs-slide-to="1"></li>
      <li data-bs-target="#carouselExampleIndicators" data-bs-slide-to="2"></li>
    </ol>
    <div class="carousel-inner">
      <div class="carousel-item active">
        <img
          src="../assets/images/slider1.png"
          class="web__img w-100"
          alt="..."
        />
        <img
          src="../assets/images/mobile1.png"
          class="mobile__img w-100"
          alt="..."
        />
        <div class="overlay"></div>
        <div class="carousel-item__content content__one">
          <img
            src="../assets/images/type-smartdelivery.png"
            class="web__title w-100"
            alt="..."
          />
          <img
            src="../assets/images/type-smartdelivery-w.png"
            class="mobile__title w-100"
            alt="..."
          />
          <p>
            It is one of the creations of smart life company that was launched
            in 2021 to be the pioneer application with easy use, simple and
            attractive design for the vendors. For more information, contact
            with Smart life company
          </p>
          <h3 class="mt-3">FOR DELIVERY</h3>
          <p>Download Application on your mobile device.</p>
          <div class="carousel__data__images mt-4">
            <img class="me-2 w-25" src="../assets/images/app-store.png" />
            <img class="me-2 w-25" src="../assets/images/app-gallaery.png" />
            <img class="w-25" src="../assets/images/google-store.png" />
          </div>
        </div>
      </div>
      <div class="carousel-item">
        <div class="carousel-item__content__second">
          <img
            src="../assets/images/type-smartdelivery.png"
            class="web__title w-100"
            alt="..."
          />
          <img
            src="../assets/images/type-smartdelivery-w.png"
            class="mobile__title w-100"
            alt="..."
          />

          <p>
            It is one of the creations of smart life company that was launched
            in 2021 to be the pioneer application with easy use, simple and
            attractive design for the vendors. For more information, contact
            with Smart life company
          </p>
          <h3 class="mt-3">FOR DELIVERY</h3>
          <p>Download Application on your mobile device.</p>
          <div class="carousel__data__images mt-4">
            <img class="me-2 w-25" src="../assets/images/app-store.png" />
            <img class="me-2 w-25" src="../assets/images/app-gallaery.png" />
          </div>
        </div>
        <img
          src="../assets/images/slider2.png"
          class="web__img w-100"
          alt="..."
        />
        <img
          src="../assets/images/mobile2.png"
          class="mobile__img w-100"
          alt="..."
        />
        <div class="overlay"></div>
      </div>
      <div class="carousel-item">
        <img
          src="../assets/images/slider3.png"
          class="web__img w-100"
          alt="..."
        />
        <img
          src="../assets/images/mobile3.png"
          class="mobile__img w-100"
          alt="..."
        />
        <div class="overlay"></div>
        <div class="carousel-item__content">
          <img
            src="../assets/images/type-smartdelivery.png"
            class="web__title w-100"
            alt="..."
          />
          <img
            src="../assets/images/type-smartdelivery-w.png"
            class="mobile__title w-100"
            alt="..."
          />

          <p>
            It is one of the creations of smart life company that was launched
            in 2021 to be the pioneer application with easy use, simple and
            attractive design for the vendors. For more information, contact
            with Smart life company
          </p>
          <h3 class="mt-3">FOR DELIVERY</h3>
          <p>Download Application on your mobile device.</p>
          <div class="carousel__data__images mt-4">
            <img class="me-2 w-25" src="../assets/images/app-store.png" />
            <img class="me-2 w-25" src="../assets/images/app-gallaery.png" />
            <img class="w-25" src="../assets/images/google-store.png" />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Carousel",
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.carousel {
  position: relative;
}

#carouselExampleIndicators {
  width: 100%;
  height: 100%;
  margin: auto;
}

.carousel-indicators {
  position: absolute;
  top: 10%;
  right: 0% !important;
  left: unset !important;
  margin-right: 10px !important;
  flex-direction: column;
}

.carousel-indicators li {
  border-radius: 50%;
  width: 6px;
  height: 6px;
  padding: 4px;
  position: relative;
  margin: 0 15px;
  background-color: transparent;
  background-color: #fff;
  opacity: 1;
}

.carousel-indicators li:after {
  border-radius: 50%;
  padding: 2px;
  border: 1px solid rgb(128, 128, 128);
  position: absolute;
  content: "";
  top: -1px;
  left: -1px;
  bottom: -1px;
  right: -1px;
}

.carousel-indicators li.active {
  background-color: #ffc107 !important;
}

.carousel-item {
  position: relative;
}
.carousel-item__content {
  position: absolute;
  top: 10%;
  right: 10%;
  width: 45%;
  text-align: left;
}
.content__one {
  animation: content 1s normal;
  transition: all 1s ease-in-out;
}

.carousel-item__content__second {
  position: absolute;
  top: 10%;
  left: 5%;
  width: 45%;
  text-align: left;
}
p {
  font-weight: 500;
}
h3 {
  font-weight: 600;
}

.mobile__img {
  display: none;
  overflow: hidden;
}
.mobile__title {
  display: none;
  overflow: hidden;
}

@keyframes content {
  0% {
    transform: translatey(900px);
    opacity: 0;
  }

  100% {
    transform: translatey(0px);
    opacity: 1;
  }
}

@media (max-width: 900px) {
  .mobile__img {
    display: block;
    overflow: visible;
    height: 100vh;
  }
  .web__img {
    display: none;
    overflow: hidden;
  }

  .carousel-item {
    color: #fff !important;
  }
  .carousel-item__content {
    width: 80%;
  }
  .carousel-item__content__second {
    color: #fff !important;
     width: 80%;
    z-index: 100;
  }

  .overlay {
    position: absolute;
    top: 0%;
    left: 0%;
    width: 100%;
    height: 100%;
    background-color: rgba(0, 0, 0, 0.568);
  }
  .web__title {
    display: none;
    overflow: hidden;
  }
  .mobile__title {
  display: block;
  overflow: visible;
}
}
</style>
