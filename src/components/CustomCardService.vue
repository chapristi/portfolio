<template>
  <div class="card-content">
    <img :src="linkImage" alt="image" />
    <h3>{{ title }}</h3>
    <p>{{ paragraph }}</p>
  </div>
</template>
<script>
export default {
  name: "CUSTOM_btn",
  props: ["title", "paragraph", "linkImage"],
};
</script>
<style lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Epilogue:wght@500;700&display=swap");

body {
  background-color: darkviolet;
}

.card-content {
  background-color: white;
  border: 0.1px solid;
  height: 400px;
  width: 350px;
  border-radius: 10px;
  font-family: "Epilogue", sans-serif;
  max-width: 350px;
  box-shadow: rgba(149, 157, 165, 0.2) 0 8px 24px;
  p {
    font-size: 19px;
    padding: 0 6% 6%;
  }
  h3 {
    font-size: 22px;
    color: #42b983;
  }
  img {
    margin-top: 10%;
  }
}
</style>
