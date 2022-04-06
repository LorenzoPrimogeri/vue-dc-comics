<template>
  <div>
    <div class="container-fluid bg-black">
      <div class="container py-4">
        <div>
          <h2 class="py-4 c-white">
            --
            <img src="../assets/img/angle-right-solid.svg" alt="right" />
            Content goes here
            <img src="../assets/img/angle-left-solid.svg" alt="left" />
            --
          </h2>
        </div>
      </div>
    </div>
    <div class="container-fluid bg-blue py-3">
      <div class="container py-3">
        <div>
          <ul>
            <li>
              <img
                class="sizeImg"
                src="../assets/img/buy-comics-digital-comics.png"
                alt="buy-comics-digital-comics.png"
              />
              DIGITAL COMICS
            </li>
            <li>
              <img
                class="sizeImg"
                src="../assets/img/buy-comics-merchandise.png"
                alt="buy-comics-merchandise.png"
              />
              DC MERCHANDISE
            </li>
            <li>
              <img
                class="sizeImg"
                src="../assets/img/buy-comics-subscriptions.png"
                alt="buy-comics-shop-locator.png"
              />
              SUBSCRIPTION
            </li>
            <li>
              <img
                class="sizeImg"
                src="../assets/img/buy-comics-shop-locator.png"
                alt="buy-comics-subscriptions.png"
              />
              COMIC SHOP LOCATOR
            </li>
            <li>
              <img
                class="sizeImg"
                src="../assets/img/buy-dc-power-visa.svg"
                alt="buy-dc-power-visa.svg"
              />
              DC POWER VISA
            </li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "MainComponent",
};
</script>

<style scoped>
h2 img {
  width: 15px;
}

.bg-blue {
  background-color: hsl(209deg 98% 49%);
}
li {
  color: white;
}
.sizeImg {
  padding-right: 5px;
  width: 40px;
}
</style>