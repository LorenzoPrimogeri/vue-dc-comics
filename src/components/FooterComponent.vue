<template>
  <div>
    <div class="container-fluid footer-bg">
      <div class="container">
        <div class="row">
          <div class="col-7 d-flex py-4">
            <ul class="d-flex flex-column">
              <li>
                <h3>DC COMICS</h3>
                <ul class="d-flex flex-column c-grey my-2 p-0">
                  <li>Characters</li>
                  <li>Coimic</li>
                  <li>Movies</li>
                  <li>TV</li>
                  <li>Games</li>
                  <li>Videos</li>
                  <li>News</li>
                </ul>
              </li>
              <li>
                <h3>SHOP</h3>
                <ul class="d-flex flex-column c-grey p-0">
                  <li>Shop DC</li>
                  <li>Shop DC Collectibles</li>
                </ul>
              </li>
            </ul>
            <ul>
              <li class="p-0">
                <h3>DC</h3>
                <ul class="d-flex flex-column c-grey my-2 p-0">
                  <li>Terms Of USe</li>
                  <li>Privacy policy (New)</li>
                  <li>Ad Choices</li>
                  <li>Advertising</li>
                  <li>Subscriptions</li>
                  <li>Talent Workshops</li>
                  <li>CPSC Certificates</li>
                  <li>Ratings</li>
                  <li>Shop Help</li>
                  <li>Contact Us</li>
                </ul>
              </li>
            </ul>
            <ul>
              <li class="p-0">
                <h3>SITES</h3>
                <ul class="d-flex flex-column c-grey my-2 p-0">
                  <li>DC</li>
                  <li>MAD Magazine</li>
                  <li>DC Kids</li>
                  <li>DC Universe</li>
                  <li>DC Power Visa</li>
                </ul>
              </li>
            </ul>
          </div>
          <div class="col-5 dc-logo"></div>
        </div>
      </div>
    </div>
    <div class="container-fluid bg-grey p-0">
      <div class="container bg-grey">
        <div class="row justify-content-between py-5">
          <div class="col-3 py-2">
            <a class="lp-btn c-white p-3" href="">SING Up NOW!</a>
          </div>
          <div class="col-9 d-flex justify-content-end">
            <h3 class="c-blue">FOLLOW US</h3>
            <div>
              <ul>
                <li>
                  <img src="../assets/img/footer-facebook.png" alt="facebook" />
                </li>
                <li>
                  <img
                    src="../assets/img/footer-periscope.png"
                    alt="periscope"
                  />
                </li>
                <li>
                  <img
                    src="../assets/img/footer-pinterest.png"
                    alt="pinterest"
                  />
                </li>
                <li>
                  <img src="../assets/img/footer-twitter.png" alt="twitter" />
                </li>
                <li>
                  <img src="../assets/img/footer-youtube.png" alt="youtube" />
                </li>
              </ul>
            </div>
          </div>
        </div>
      </div>
      <div class="space bg-black"></div>
    </div>
  </div>
</template>

<script>
export default {
  name: "FooterComponent",
};
</script>

<style scoped>
.footer-bg {
  background-image: url("../assets/img/footer-bg.jpg");
  background-size: cover;
}
.dc-logo {
  background-image: url("../assets/img/dc-logo-bg-adattata.png");
  background-size: cover;
}
li h3 {
  color: white;
}
.space {
  height: 30px;
}
.bg-grey {
  background-color: hsl(0deg 0% 19%);
}
.c-blue {
  color: blue;
}
.lp-btn {
  border: 1px solid hsl(209deg 98% 49%);
  font-weight: 700;
}
</style>