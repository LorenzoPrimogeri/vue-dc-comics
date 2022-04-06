<template>
  <div>
    <div class="container-fluid footer-bg">
      <div class="container">
        <div class="row py-5">
          <div class="col-7 d-flex">
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
          <div class="col-5"></div>
        </div>
      </div>
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
}
li h3 {
  color: white;
}
</style>