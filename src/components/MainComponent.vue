<template>
  <div>
    <div class="container-fluid bg-blue py-3">
      <div class="container py-3">
        <div>
          <ul class="d-flex justify-content-between align-items-center">
            <li v-for="element in dcIcon" :key="element">
              <img class="sizeImg" :src="element.icon" :alt="element.name" />
              {{ element.name }}
            </li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import dcIcon from "../assets/data/dcIcondata";
export default {
  name: "MainComponent",
  data() {
    return {
      dcIcon,
    };
  },
};
</script>

<style scoped>
.bg-blue {
  background-color: hsl(209deg 98% 49%);
}
li {
  color: white;
}
.sizeImg {
  padding-right: 5px;
  width: 60px;
}
</style>