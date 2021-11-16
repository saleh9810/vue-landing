<template>
<footer class="">
    <div class="footer__content d-flex justify-content-between  align-items-center container">
        <div class="footer__content__box">
            @ 2021 Samrt delivery 
            <img src="../assets/images/smartlife-footer.png" alt="">
        </div>
        <div id="nav">
            <router-link class="nav__link" to="/about">About</router-link>
            <router-link to="/policy">policy</router-link>
  </div>
    </div>

</footer>
    
</template>

<script>
export default {
   name: "Footer"
}
</script>

<style scoped>
footer {
    background-color: rgb(0, 0, 0);
    padding: 10px 20px;
    position: fixed;
    bottom: 0;
    width: 100%;

}
.footer__content__box {
    color: #fff;
}
.nav {
    color: #fff;
    
}
 a {
    text-decoration: none;
    color: #fff;
    margin: 0 5px;

}
.nav__link::after {
    content: "|";
    padding-left: 10px;

}

@media (max-width: 900px) {
 img {
     width: 40%;
 }
}

@media (max-width: 700px) {
 a {
 }
}


</style>


