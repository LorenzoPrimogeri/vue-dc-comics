<template>
  <div class="container-fluid bg-black">
    <div class="container p-0">
      <div class="row justify-content-between g-1">
        <div v-for="element in dcComics" :key="element" class="col">
          <div>
            <img :src="element.thumb" :alt="element.thumb" />
          </div>
          <div>
            <p class="m-0 c-white">{{ element.series }}</p>
            <div class="d-flex flex-column">
              <a class="c-grey" href="">{{ element.type }}</a>
              <a class="c-red" href="">{{ element.price }}</a>
            </div>
          </div>
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
</style>