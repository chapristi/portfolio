<template>
  <div v-on:click="hidden1" class="question">
    <p>Create a Webinar in Minutes +</p>
  </div>
  <div v-if="!this.isHidden1" class="response">
    <p>
      Interdum velit euismod in pellentesque massa placerat duis. Tristique et
      egestas quis ipsum suspendisse ultrices gravida dictum fusce. Nibh nisl
      condimentum.
    </p>
  </div>
  <div v-on:click="hidden2" class="question">
    <p>Create a Webinar in Minutes +</p>
  </div>
  <div v-if="!this.isHidden2" class="response">
    <p>
      –Interdum velit euismod in pellentesque massa.<br />
      –Tristique et egestas quis ipsum suspendisse ultrices gravidae. <br />
      –Nibh nisl
      <br />
      condimentum id venenatis a condimentum. –Diam volutpat commodo sed egestas
      egestas fringilla.
    </p>
  </div>
  <div v-on:click="hidden3" class="question">
    <p>Create a Webinar in Minutes +</p>
  </div>
  <div v-if="!this.isHidden3" class="response">
    <p>
      Interdum velit euismod in pellentesque massa placerat duis. Tristique et
      egestas quis ipsum suspendisse ultrices gravida dictum fusce. Nibh nisl
      condimentum.
    </p>
  </div>
  <div v-on:click="hidden4" class="question">
    <p>Create a Webinar in Minutes +</p>
  </div>
  <div v-if="!this.isHidden4" class="response">
    <p>
      Interdum velit euismod in pellentesque massa placerat duis. Tristique et
      egestas quis ipsum suspendisse ultrices gravida dictum fusce. Nibh nisl
      condimentum.
    </p>
  </div>
</template>
<script>
export default {
  name: "suposedQuestions",
  data: function () {
    return {
      isHidden1: true,
      isHidden2: true,
      isHidden3: true,
      isHidden4: true,
    };
  },
  methods: {
    hidden1: function () {
      this.isHidden1 = !this.isHidden1;
    },
    hidden2: function () {
      this.isHidden2 = !this.isHidden2;
    },
    hidden3: function () {
      this.isHidden3 = !this.isHidden3;
    },
    hidden4: function () {
      this.isHidden4 = !this.isHidden4;
    },
  },
};
</script>

<style lang="scss">
.response {
  margin-left: 25%;
  width: 60%;
  height: 25% !important;
  text-align: left;

  p {
    color: whitesmoke;
  }
}
.question {
  border: 0.1px solid;
  box-shadow: rgba(0, 0, 0, 0.05) 0 6px 24px 0, rgba(0, 0, 0, 0.08) 0 0 0 1px;
  margin-left: 20%;
  background-color: greenyellow;
  width: 70%;
  height: 15% !important;
  &:first-child {
    border-radius: 10px 10px 0 0;
  }
  &:last-child {
    border-radius: 0 0 10px 10px;
  }
  &:hover {
    background-color: yellow;
  }
  p {
    margin: auto;
  }
}
</style>
