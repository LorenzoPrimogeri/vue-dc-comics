<template>
  <div class="container-fluid">
    <div class="space bg-black"></div>
    <div class="container">
      <div class="row justify-content-betweeen py-3">
        <div class="col-2">
          <img src="../assets/img/dc-logo.png" alt="dc-logo.png" />
        </div>
        <div class="col-10 d-flex align-items-center justify-content-end">
          <ul>
            <li v-for="(element, index) in links" :key="index">
              {{ element }}
            </li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "HeaderComponent",
  props: ["links"],
};
</script>

<style scoped>
.space {
  height: 30px;
}
li {
  font-weight: 700;
}
.container-fluid {
  padding: 0;
}
</style>