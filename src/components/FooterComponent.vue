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
                  <li v-for="element in links" :key="element">{{ element }}</li>
                </ul>
              </li>
              <li>
                <h3>SHOP</h3>
                <ul class="d-flex flex-column c-grey p-0">
                  <li v-for="element in shop" :key="element">{{ element }}</li>
                </ul>
              </li>
            </ul>
            <ul>
              <li class="p-0">
                <h3>DC</h3>
                <ul class="d-flex flex-column c-grey my-2 p-0">
                  <li v-for="element in dc" :key="element">{{ element }}</li>
                </ul>
              </li>
            </ul>
            <ul>
              <li class="p-0">
                <h3>SITES</h3>
                <ul class="d-flex flex-column c-grey my-2 p-0">
                  <li v-for="element in sites" :key="element">{{ element }}</li>
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
            <a class="lp-btn c-white p-3" href="">SIGN UP NOW!</a>
          </div>
          <div class="col-9 d-flex justify-content-end">
            <h3 class="c-blue">FOLLOW US</h3>
            <div>
              <ul>
                <li v-for="element in socialMediaData" :key="element">
                  <img :src="element.icon" :alt="element.name" />
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
import socialMediaData from "../assets/img/socialMediaData";
export default {
  name: "FooterComponent",
  props: ["links".toLowerCase()],
  data() {
    return {
      shop: ["Shop DC", "Shop DC Collectibles"],
      dc: [
        "Terms Of USe",
        "Privacy policy (New)",
        "Ad Choices",
        "Advertising",
        "Subscriptions",
        "Talent Workshops",
        "CPSC Certificates",
        "Ratings",
        "Shop Help",
        "Contact Us",
      ],
      sites: ["DC", "MAD Magazine", "DC Kids", "DC Universe", "DC Power Visa"],
      socialMediaData,
    };
  },
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