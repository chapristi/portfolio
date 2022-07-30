<template>
  <!--<div class="home">
    <div class="hero__banner">
      <div class="txt">
        <h1>Webdev Services</h1>
        <p>
          Pharetra convallis posuere morbi leo. <br />
          Tellus mauris a diam maecenas.
        </p>
        <p>Image from <span class="outline">Freepik</span></p>
        <button class="btn_contact">contact us</button>
      </div>
      <div class="picture">
        <img
          src="https://developer.mozilla.org/assets/mdn_contributor.png"
          alt="un picture"
        />
      </div>
    </div>
  </div>-->
  <div class="home">

  </div>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from "@/components/HelloWorld.vue";

const paper = require('paper');
console.log(paper)

export default {
  name: "Home",
  components: {
    // HelloWorld,
  },
};
</script>

<style lang="scss" scoped>
@import "./src/assets/styles/components";

.hero__banner {
  display: flex;
  align-items: center;
  justify-content: space-around;
  height: 80vh;
  background-color: #2a2a2a;
  h1 {
    font-size: 52px;
    font-weight: bold;
    color: #31ff1e;
  }
  p {
    font-size: 22px;
    color: #31c81e;
  }
  .txt {
    display: grid;
    grid-gap: 20px;
    grid-template-columns: repeat(1, 4fr);
/*    h1,
    p,
    button {
      grid-column: 1/4;
      grid-row: 1;
    }*/
  }
}
</style>
