<template>
       <!-- Start Header -->
        <header class="header">
            <div class="container">
                <div class="row">
                    <div class="col-lg-6 col-md-4 col-sm-4 col-3">
                      <router-link to="/">
                        <img src="../assets/images/logo-SmartDelivery.png" class="logo">
                      </router-link>
                    </div>
                    <div class="col-lg-6 col-md-8 col-sm-8 col-9 align-self-center">
                        <nav class="nav social-icon-nav justify-content-end">
                            <a class="nav-link" href="#"><i class="fab fa-facebook-f"></i></a>
                            <a class="nav-link" href="#"><i class="fab fa-twitter"></i></a>
                            <a class="nav-link" href="#"><i class="fab fa-instagram"></i></a>
                            <a class="nav-link" href="#"><i class="fab fa-youtube"></i></a>
                            <a href="#" class="login-btn">Login</a>
                        </nav>
                    </div>
                </div>
            </div>
        </header>
</template>

<script>
export default {
  name: "Navbar",
};
</script>

<style scoped>
.header {
  background-color: #ffc107;
}
.navbar-nav {
  align-items: center;
}
 .nav-link {
  background: #fff;
  color: #000 !important;
  margin: 0 0.4rem;
  border-radius: 50%;
  padding-right: 0.9rem !important;
  padding-left: 0.9rem !important;
  font-size: 1.2rem;
  transition: all 0.2s ease-in-out;
}
 .nav-link:hover {
    background: #000;
      color: #ffc107 !important;
}

 .login-btn {
  text-decoration: none;
  font-size: 1.2rem;
  background-color: #000;
  padding: 0.6rem 1.9rem;
  border-radius: 25px;
  color: #ffc107;
  transition: all 0.2s ease-in-out;
  text-transform: uppercase;
}
 .login-btn:hover {
    background-color: rgb(255, 255, 255);

}

@media (max-width: 900px) {
  :root {
    font-size: 10px;
  }
   img {
    width: 100%;
  }
  .header {
    padding: 1rem;
}
}



</style>
