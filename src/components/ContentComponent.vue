<template>
  <div>
    <div class="container-fluid jt-image">
    </div>
    <div class="container-fluid bg-black">
      <div class="container p-0 position-relative">
        <p class="lp-btn bg-blue c-white position-absolute">CURRENT SERIES</p>
        <div class="row justify-content-between g-1 py-5">
          <div
            v-for="(element, index) in dcComics"
            :key="index"
            class="col d-flex flex-wrap"
          >
            <div>
              <img :src="element.thumb" :alt="element.thumb" />
            </div>
            <div class="d-flex flex-wrap">
              <p class="m-0 c-white w-100">{{ element.series }}</p>
              <div class="d-flex flex-column align-self-end">
                <a class="c-grey" href="">{{ element.type }}</a>
                <a class="c-red" href="">{{ element.price }}</a>
              </div>
            </div>
          </div>
        </div>
        <div class="text-center py-3">
          <a class="c-white lp-btn bg-blue" href="">Load More</a>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import dcComics from "../assets/data/dc-comics";
export default {
  name: "ContentComponent",
  data() {
    return {
      dcComics,
    };
  },
};
</script>

<style scoped>
p {
  font-size: 20px;
}
.lp-btn {
  border: 1px solid white;
  padding: 5px 40px;
}
.jt-image {
  background-image: url("../assets/img/jumbotron.jpg");
  height: 400px;
  background-size: cover;
  background-repeat: no-repeat;
}
.position-relative p{
  top: -20px;
}
</style>