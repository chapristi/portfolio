<template>
  <div class="test">
    <img :src="link" />
  </div>
</template>
<script>
export default {
  props: ["link"],
};
</script>
<style lang="scss">
.test {
  background-color: blueviolet;
  height: 350px;
  width: 70%;
  border-radius: 10px;
  margin-left: 25%;
  img {
    margin-top: 5%;
    height: 80%;
    width: 80%;
    border-radius: 10px;
  }
}
</style>
